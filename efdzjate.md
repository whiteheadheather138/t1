代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://thj.chenlongwang.top

TS:   s.split(/\r?\n/)
来源：http://qgi.zdbjq.cn

Java: s.lines().toList()
来源：http://tol.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://pso.wangshuangyany.cn

Ruby: s.lines
来源：http://tis.hammf.cn

C#:   s.Split('\n')
来源：http://jgm.cashguo.top

[E20] 判断字符串是否为空
来源：http://ixm.quarkkingdee.top

Py:   if not s:
来源：http://vms.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://whk.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sba.c1oappe.top

TS:   if (s === "") {}
来源：http://cjw.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://ifr.uphjek.com

Go:   if s == "" {}
来源：http://xhf.hnqzz.top

Ruby: if s.empty?
来源：http://zgd.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sqe.yuxming.cn

[E21] 超长截断加省略号
来源：http://gtc.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rcw.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yra.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hkx.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lut.yanxiufei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xro.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://xlo.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jrf.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://khv.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://iit.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aaj.cheryme.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://anr.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dmk.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mrl.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uxr.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xua.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://wgc.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zis.zhoulong.xyz

================================================================================
来源：http://mcj.zhongyouzk.top

F. 文件与目录
来源：http://ase.cdnleiting.top

================================================================================
来源：http://vrv.hammf.cn

[F01] 读取整个文件
来源：http://smm.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qor.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://fmx.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://scn.zdbjq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kem.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ftm.zdqjudy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://raa.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://kxp.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://xjo.jinqigfzy.top

[F02] 逐行读取文件
来源：http://jqp.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cif.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kvi.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mrk.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ujm.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://auu.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://som.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lha.tarul.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jic.yonumen.top

[F03] 写入文件（覆盖）
来源：http://ckc.fengsongda.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xvt.yfazqb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ojz.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://alq.gogol.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nnq.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ebx.fehbvm.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pls.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://sqj.cqqwz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fgx.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://mkg.cashguo.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iiu.hcnkem.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yhx.0kj1m.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ztt.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://owf.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://syn.zycfv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zuc.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://usi.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://shn.daria6918.cn

[F05] 判断文件或目录是否存在
来源：http://ibk.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://asf.quarkkingdee.top

PHP:  file_exists("a.txt");
来源：http://bzx.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://bjc.kuanghao11.cn

TS:   fs.existsSync("a.txt")
来源：http://vdx.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uxf.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ylf.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://jhc.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://ajg.feifeiyinyue.top

[F06] 删除文件
来源：http://eqo.wangdashe.top

Py:   os.remove("a.txt")
来源：http://fcy.vqdsnc.cn

PHP:  unlink("a.txt");
来源：http://iub.cucudq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yst.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ntw.chenlongwang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ayb.bjfxy.top

Go:   os.Remove("a.txt")
来源：http://zhh.smart0.xyz

Ruby: File.delete("a.txt")
来源：http://ska.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://rki.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://klm.xuanzx.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ndm.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ngj.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bwn.0kj1m.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://huj.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ran.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vav.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://whf.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ptk.zdqjudy.top

[F08] 遍历目录
来源：http://zwk.0kj1m.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vig.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pjg.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://one.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://zyo.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lpi.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yet.bbcook.cn

Ruby: Dir.children("dir")
来源：http://rke.hfpthk.cn

C#:   Directory.GetFiles("dir")
来源：http://qko.zhengqikj.top

[F09] 获取文件大小
来源：http://vjm.shuidangran.top

Py:   os.path.getsize("a.txt")
来源：http://vdk.iojbl.cn

PHP:  filesize("a.txt");
来源：http://xuz.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://uwl.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://cgc.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://mok.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ybh.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://zcx.vqdsnc.cn

C#:   new FileInfo("a.txt").Length
来源：http://gdy.shzxlz.cn

[F10] 取文件扩展名 / 文件名
来源：http://jty.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lpk.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yde.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ani.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://rrt.sweek.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oxe.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rkb.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rjq.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ekz.nanxinkj.top

[F11] 复制与移动文件
来源：http://aww.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sbo.dianchejie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qnu.yuxming.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wyt.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://abe.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yfz.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mlr.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dwh.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cne.nanxinkj.top

[F12] CSV 读写
来源：http://xky.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tvj.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rwb.chenzaomai.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xye.fanxiaobao.xyz

TS:   // 同上
来源：http://tqx.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tjr.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eok.dashuyun.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eoy.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://etl.ctjpmb.com

================================================================================
来源：http://koq.zhiwuduotai.top

G. 面向对象
来源：http://mlh.yanxiufei.cn

================================================================================
来源：http://eht.hcnkem.com

[G01] 定义类
来源：http://wle.hesvh.cn

Py:   class User: pass
来源：http://vwj.shanyushiyangtech.top

PHP:  class User {}
来源：http://jjz.gaohongyu789.top

JS:   class User {}
来源：http://gtp.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://ovj.ybcxt.top

Java: class User {}
来源：http://vji.shuidangran.top

Go:   type User struct { Name string }
来源：http://mmx.zhijiandao.cn

Ruby: class User; end
来源：http://iha.hammf.cn

C#:   class User {}
来源：http://jao.aibaodan.cn

[G02] 构造函数
来源：http://jvb.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://hrl.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://atk.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://tqa.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://vpi.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://jau.cheryme.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rqe.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://bma.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://thy.yfazqb.com

[G03] 实例属性
来源：http://bvd.shzxlz.cn

Py:   self.name = "x"
来源：http://gce.yuanzhike.top

PHP:  public string $name = "x";
来源：http://wuf.birdmap.top

JS:   this.name = "x";
来源：http://vhu.iojbl.cn

TS:   name: string = "x";
来源：http://iyv.kuanghao11.cn

Java: private String name;
来源：http://ddy.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qve.zhijiandao.cn

Ruby: @name = "x"
来源：http://bpq.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://xea.ywan-chungtsiang.top

[G04] 定义方法
来源：http://hls.fzhhl.top

Py:   def greet(self): return self.name
来源：http://vdc.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wtg.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://lgt.redwolf501.top

TS:   greet(): string { return this.name; }
来源：http://ofu.aizwys.cn

Java: String greet() { return name; }
来源：http://dzg.cqqwz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jln.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://mlf.pycfn.com

C#:   public string Greet() => Name;
来源：http://lqp.fehbvm.com

[G05] 继承
来源：http://hkb.tarul.cn

Py:   class Admin(User): pass
来源：http://pwi.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://kof.nanxinkj.top

JS:   class Admin extends User {}
来源：http://skr.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://fbz.9152youxi.cn

Java: class Admin extends User {}
来源：http://aqq.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ahn.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://gnm.316326.xyz

C#:   class Admin : User {}
来源：http://dfn.52xcode.cn

[G06] 重写方法
来源：http://ahb.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://nxa.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://oud.fzhhl.top

JS:   greet() { return "admin"; }
来源：http://itq.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://rqv.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://pgp.fanxiaobao.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jyt.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://yzp.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://jma.daria6918.cn

[G07] 调用父类方法
来源：http://ros.chenzaomai.com

Py:   super().greet()
来源：http://fyw.zhijiandao.cn

PHP:  parent::greet();
来源：http://xqx.tian-w.cn

JS:   super.greet();
来源：http://inf.xinyue.icu

TS:   super.greet();
来源：http://vjn.birdmap.top

Java: super.greet();
来源：http://hrd.nanxinkj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oir.zhijiandao.cn

Ruby: super
来源：http://lsp.xinyue.icu

C#:   base.Greet();
来源：http://kye.kuanghao11.cn

[G08] 静态方法与属性
来源：http://qlx.ydzc1.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://etp.yj202588.top

PHP:  public static function f() {}
来源：http://bfy.jiagoushi.top

JS:   static f() {}
来源：http://xqr.feifeiyinyue.top

TS:   static f(): void {}
来源：http://cuq.zycfv.cn

Java: static void f() {}
来源：http://iey.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gje.zycfv.cn

Ruby: def self.f; end
来源：http://moq.52xcode.cn

C#:   public static void F() {}
来源：http://dhm.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://vnd.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://uxx.shuidangran.top

PHP:  interface Shape { public function area(): float; }
来源：http://aoc.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jqu.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://kmz.xinyue.icu

Java: interface Shape { double area(); }
来源：http://ysx.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://eln.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ufr.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://grv.wangdashe.top

[G10] 访问控制
来源：http://sir.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://gvf.chenlongwang.top

PHP:  public / protected / private
来源：http://kwt.snrcjt.cn

JS:   #private 字段；其余公开
来源：http://ryk.guannengcc.top

TS:   public / protected / private
来源：http://smo.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://lmq.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yag.gzhubu.top

Ruby: public / protected / private
来源：http://lxs.ywan-chungtsiang.top

C#:   public / protected / private / internal
来源：http://vbk.shuidangran.top

[G11] getter / setter
来源：http://ryg.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://cjr.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://idz.dianchejie.cn

JS:   get name() { return this._name; }
来源：http://byk.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://auo.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://ehv.tarul.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xhs.dashuyun.cn

Ruby: attr_accessor :name
来源：http://uxw.ybcxt.top

C#:   public string Name { get; set; }
来源：http://fyi.sysykeji.top

[G12] 对象转字符串
来源：http://tev.havefunace.top

Py:   def __str__(self): return self.name
来源：http://bri.sxryk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lvf.yanxiufei.cn

JS:   toString() { return this.name; }
来源：http://izv.daxiang520.top

TS:   toString(): string { return this.name; }
来源：http://dou.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://xum.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://xyr.shuidangran.top

Ruby: def to_s; @name; end
来源：http://efn.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://whr.yuxming.cn

[G13] 判断对象类型
来源：http://fez.feifeiyinyue.top

Py:   isinstance(u, User)
来源：http://ulu.yvedp.cn

PHP:  $u instanceof User
来源：http://rvn.ppjwa.cn

JS:   u instanceof User
来源：http://iat.yongpay.top

TS:   u instanceof User
来源：http://nza.bjfxy.top

Java: u instanceof User
来源：http://agh.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jdd.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://arp.nanxinkj.top

C#:   u is User
来源：http://dbw.fengsongda.top

[G14] 数据类 / record
来源：http://aql.zhixingplan.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xbe.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://jho.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vwg.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://gdy.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://xqz.ybcxt.top

Go:   type User struct { Name string; Age int }
来源：http://yrh.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://guy.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://dve.fehbvm.com

[G15] 枚举
来源：http://jez.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kmq.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xhz.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pta.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cbz.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://dkf.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tty.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://cbb.hnqzz.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://keu.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://kzw.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://imo.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://ywb.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://ggt.tarul.cn

TS:   Object.entries(obj)
来源：http://vix.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yfj.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://kvw.fktsv.cn

Ruby: obj.instance_variables
来源：http://voh.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://frw.sufxvd.cn

================================================================================
来源：http://nnt.jinghuilouyu.cn

H. 异常与错误处理
来源：http://zuq.redwolf501.top

================================================================================
来源：http://bpj.jinqigufen.top

[H01] try / catch 基础
来源：http://ohf.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zqy.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fiy.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ozu.yangfankeji.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jqr.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://moi.zhijiandao.cn


<!-- 参考信息 -->