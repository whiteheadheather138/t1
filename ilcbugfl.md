代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wjo.xuanzx.com

[E19] 多行文本按行拆分
来源：http://jhp.smart0.xyz

Py:   s.splitlines()
来源：http://qao.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://buj.zhijiandao.cn

JS:   s.split(/\r?\n/)
来源：http://qdm.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://tui.zhengqikj.top

Java: s.lines().toList()
来源：http://tie.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://ewm.9152youxi.cn

Ruby: s.lines
来源：http://eup.xuanzx.com

C#:   s.Split('\n')
来源：http://lub.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://ool.birdmap.top

Py:   if not s:
来源：http://ffi.gzhubu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dph.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xsf.quarkkingdee.top

TS:   if (s === "") {}
来源：http://ved.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://nve.daxiang520.top

Go:   if s == "" {}
来源：http://cen.kuanghao11.cn

Ruby: if s.empty?
来源：http://vai.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sst.jyoumei.cn

[E21] 超长截断加省略号
来源：http://guz.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ula.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lej.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ugo.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fau.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ane.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://hzm.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tme.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wkd.yj20258.top

[E22] 字节长度与字符长度
来源：http://zif.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jql.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rnr.yj20258888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://leo.fehbvm.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lgh.fzhhl.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xpg.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jvm.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://zgs.bbcook.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vdl.jlsjyb.cn

================================================================================
来源：http://dgv.nanxinkj.top

F. 文件与目录
来源：http://pck.yonumen.top

================================================================================
来源：http://wez.ybcxt.top

[F01] 读取整个文件
来源：http://bcv.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uxu.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://sij.ehwqpu.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tzi.shanyushiyangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://aox.gogol.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zov.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ptc.epnwcf.com

Ruby: File.read("a.txt")
来源：http://tde.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://uee.ybcxt.top

[F02] 逐行读取文件
来源：http://eri.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bfn.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pjy.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ddl.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cae.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bsn.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yrq.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eho.feifeiyinyue.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kgv.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://kbv.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vku.andypj.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://fsk.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rym.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://keh.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pbf.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://plo.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://dcs.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dac.gotoacloud.top

[F04] 追加写入文件
来源：http://gmz.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oxc.fengsongda.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sxj.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fjc.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tbn.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ujj.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sow.shanyushiyangtech.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://amv.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://urn.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://yau.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uju.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://kvg.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://mni.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://mjf.kuanghao11.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qow.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://equ.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://ckk.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://cmb.xinyue.icu

[F06] 删除文件
来源：http://mbq.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://tbr.xylfe.cn

PHP:  unlink("a.txt");
来源：http://brr.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://tol.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jbx.zhaomingkeji.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qqg.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://qrl.guannengcc.top

Ruby: File.delete("a.txt")
来源：http://djo.316326.xyz

C#:   File.Delete("a.txt");
来源：http://spa.nwbrower.top

[F07] 创建目录（含多级）
来源：http://til.birdmap.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://khi.tian-w.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fta.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://toc.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oqf.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sqb.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rav.cqqwz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cbp.zhongyouzk.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tuu.52xcode.cn

[F08] 遍历目录
来源：http://nzo.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://duw.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jjj.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://xqv.vqdsnc.cn

TS:   fs.readdirSync("dir")
来源：http://tmg.hongshengwenyu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fqp.sufxvd.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wtb.guannengcc.top

Ruby: Dir.children("dir")
来源：http://mce.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://qvg.zhengqikj.top

[F09] 获取文件大小
来源：http://crh.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://jvs.mhx1999.top

PHP:  filesize("a.txt");
来源：http://riw.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://aqk.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://dst.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fqh.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nni.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://qzk.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://ind.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://gwh.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://inc.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ikc.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rbs.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://rld.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pzn.jinghuilouyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cqf.uphjek.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rkq.wangdashe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ptw.aibaodan.cn

[F11] 复制与移动文件
来源：http://lav.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pvm.cdnleiting.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bju.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cpl.0kj1m.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://awc.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ezy.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wdl.ctjpmb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wtg.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aty.bbcook.cn

[F12] CSV 读写
来源：http://izq.cashguo.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yrj.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gij.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jtb.hfpthk.cn

TS:   // 同上
来源：http://ziv.zhoulong.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wda.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vgc.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wbs.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zor.wangdashe.top

================================================================================
来源：http://wzc.xziqi.cn

G. 面向对象
来源：http://kzz.zdqjudy.top

================================================================================
来源：http://trf.jyoumei.cn

[G01] 定义类
来源：http://tpl.yongpay.top

Py:   class User: pass
来源：http://fce.ivvv.top

PHP:  class User {}
来源：http://aqe.wangdashe.top

JS:   class User {}
来源：http://pst.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://new.smart0.xyz

Java: class User {}
来源：http://wfv.mhx1999.top

Go:   type User struct { Name string }
来源：http://dqc.meibo888.top

Ruby: class User; end
来源：http://omb.zhijiandao.cn

C#:   class User {}
来源：http://cio.gzhubu.top

[G02] 构造函数
来源：http://qic.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://dvq.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://glv.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://dbh.316326.xyz

TS:   constructor(public name: string) {}
来源：http://lom.zhongyouzk.top

Java: User(String name) { this.name = name; }
来源：http://cdg.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mgn.hesvh.cn

Ruby: def initialize(name); @name = name; end
来源：http://eqz.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://tfi.zdqjudy.top

[G03] 实例属性
来源：http://gwy.nwbrower.top

Py:   self.name = "x"
来源：http://pho.sweek.top

PHP:  public string $name = "x";
来源：http://gvt.bjfxy.top

JS:   this.name = "x";
来源：http://rka.yuanzhike.top

TS:   name: string = "x";
来源：http://ujx.snrcjt.cn

Java: private String name;
来源：http://ypm.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yzj.bjfxy.top

Ruby: @name = "x"
来源：http://xqu.zdqjudy.top

C#:   public string Name { get; set; } = "x";
来源：http://qfh.kuanghao11.cn

[G04] 定义方法
来源：http://rjd.fzhhl.top

Py:   def greet(self): return self.name
来源：http://ylv.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jrn.jinyuanbaomall.cn

JS:   greet() { return this.name; }
来源：http://zur.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://bvs.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://ljl.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gzu.ppjwa.cn

Ruby: def greet; @name; end
来源：http://avn.epnwcf.com

C#:   public string Greet() => Name;
来源：http://dlj.yfazqb.com

[G05] 继承
来源：http://dou.hnxiangtu.top

Py:   class Admin(User): pass
来源：http://jud.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://cfw.jiagoushi.top

JS:   class Admin extends User {}
来源：http://pyw.bbcook.cn

TS:   class Admin extends User {}
来源：http://wgz.gzhubu.top

Java: class Admin extends User {}
来源：http://sij.ivvv.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xrv.tarul.cn

Ruby: class Admin < User; end
来源：http://dri.nwbrower.top

C#:   class Admin : User {}
来源：http://utu.ybcxt.top

[G06] 重写方法
来源：http://lrq.pycfn.com

Py:   def greet(self): return "admin"
来源：http://cgn.zhaomingkeji.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://ysc.gaohongyu789.top

JS:   greet() { return "admin"; }
来源：http://ccd.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://ehn.hcnkem.com

Java: @Override String greet() { return "admin"; }
来源：http://ybk.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gwz.kuanghao11.cn

Ruby: def greet; "admin"; end
来源：http://znv.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://hvg.xylfe.cn

[G07] 调用父类方法
来源：http://ssj.chenlongwang.top

Py:   super().greet()
来源：http://put.yj20258.top

PHP:  parent::greet();
来源：http://kxz.sxryk.cn

JS:   super.greet();
来源：http://lov.jinqigufen.top

TS:   super.greet();
来源：http://cnf.yj20258888.top

Java: super.greet();
来源：http://tjg.zycfv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tpn.dianchejie.cn

Ruby: super
来源：http://ftl.zhiwuduotai.top

C#:   base.Greet();
来源：http://ofe.fengsongda.top

[G08] 静态方法与属性
来源：http://ktx.snrcjt.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dlw.yj202588.top

PHP:  public static function f() {}
来源：http://jyl.jinghuilouyu.cn

JS:   static f() {}
来源：http://rsl.aizwys.cn

TS:   static f(): void {}
来源：http://yqg.zhaomingkeji.xyz

Java: static void f() {}
来源：http://hma.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tpo.yuanzhike.top

Ruby: def self.f; end
来源：http://xgr.hysaishi.cn

C#:   public static void F() {}
来源：http://ltg.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://xsx.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://eig.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vnz.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sgy.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://wqn.daxiang520.top

Java: interface Shape { double area(); }
来源：http://ljx.sxryk.cn

Go:   type Shape interface { Area() float64 }
来源：http://wae.zdqjudy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jfu.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://qhu.zhengqikj.top

[G10] 访问控制
来源：http://dvp.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://sif.fzhhl.top

PHP:  public / protected / private
来源：http://iew.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://czz.zhoulong.xyz

TS:   public / protected / private
来源：http://stu.sweek.top

Java: public / protected / private / 默认包级
来源：http://ekg.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://daa.nanxuanxn.top

Ruby: public / protected / private
来源：http://crk.daria6918.cn

C#:   public / protected / private / internal
来源：http://ohz.fengsongda.top

[G11] getter / setter
来源：http://wsc.cashguo.top

Py:   @property 与 @x.setter
来源：http://hlh.zhongyouzk.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ley.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://dnq.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://onb.xylfe.cn

Java: public String getName() { return name; }
来源：http://erl.nanxuanxn.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qvx.jianghu66.top

Ruby: attr_accessor :name
来源：http://imu.yvedp.cn

C#:   public string Name { get; set; }
来源：http://tlm.c1oappe.top

[G12] 对象转字符串
来源：http://obh.gaohongyu789.top

Py:   def __str__(self): return self.name
来源：http://onn.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dma.fanxiaobao.xyz

JS:   toString() { return this.name; }
来源：http://wxo.yvedp.cn

TS:   toString(): string { return this.name; }
来源：http://doo.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://ajt.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rom.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://jtr.shanyushiyangtech.top

C#:   public override string ToString() => Name;
来源：http://xgp.andypj.xyz

[G13] 判断对象类型
来源：http://xcg.tanke756.top

Py:   isinstance(u, User)
来源：http://pmg.cqqwz.cn

PHP:  $u instanceof User
来源：http://jlg.zycfv.cn

JS:   u instanceof User
来源：http://iko.xylfe.cn

TS:   u instanceof User
来源：http://dpl.nwbrower.top

Java: u instanceof User
来源：http://dui.sjlbkw.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wyj.c1oappe.top

Ruby: u.is_a?(User)
来源：http://nvr.iojbl.cn

C#:   u is User
来源：http://wxo.hysaishi.cn

[G14] 数据类 / record
来源：http://zsd.jinqigfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ytc.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://mov.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vky.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://hic.zhijiandao.cn

Java: record User(String name, int age) {}
来源：http://dcm.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://xes.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://are.havefunace.top

C#:   record User(string Name, int Age);
来源：http://mjx.yuxming.cn

[G15] 枚举
来源：http://cae.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vun.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://abv.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cuf.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aim.fengsongda.top

Java: enum Color { RED, GREEN }
来源：http://rir.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qur.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://lll.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ffm.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://jkg.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mwz.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://eqw.jyoumei.cn

JS:   Object.entries(obj)
来源：http://bnc.cdnleiting.top

TS:   Object.entries(obj)
来源：http://nwd.sweek.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vjr.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ivf.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://jap.birdmap.top

C#:   // 用反射或 System.Text.Json
来源：http://mxe.zdbjq.cn

================================================================================
来源：http://wwx.chenlongwang.top

H. 异常与错误处理
来源：http://kwq.fengsongda.top

================================================================================
来源：http://wlc.gogol.net.cn

[H01] try / catch 基础
来源：http://ghu.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blz.jyoumei.cn


<!-- 参考信息 -->