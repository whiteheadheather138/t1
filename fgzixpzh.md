代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://qmc.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://azp.hnqzz.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://acv.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qht.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xuw.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://qie.kuanghao11.cn

Py:   s.splitlines()
来源：http://kwm.hcnkem.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bbj.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://pvn.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://fux.sysykeji.top

Java: s.lines().toList()
来源：http://bhe.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://drg.birdmap.top

Ruby: s.lines
来源：http://zay.daxiang520.top

C#:   s.Split('\n')
来源：http://unh.chenlongwang.top

[E20] 判断字符串是否为空
来源：http://qym.sjlbkw.cn

Py:   if not s:
来源：http://dzb.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yyz.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qdq.jianghu66.top

TS:   if (s === "") {}
来源：http://nbr.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://jbr.hcnkem.com

Go:   if s == "" {}
来源：http://rch.chenzaomai.com

Ruby: if s.empty?
来源：http://mch.zdbjq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pvo.fzhhl.top

[E21] 超长截断加省略号
来源：http://nbd.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tib.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xee.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zcd.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://scx.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mwq.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://len.yanxiufei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gia.c1oappe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rtz.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://vuz.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bdr.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sei.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wly.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cml.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bte.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lcc.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://cdg.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oai.tianlin.xyz

================================================================================
来源：http://gtu.yuxming.cn

F. 文件与目录
来源：http://miz.hesvh.cn

================================================================================
来源：http://mig.yuanzhike.top

[F01] 读取整个文件
来源：http://bpi.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fnx.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://ygf.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sbw.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vzc.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kev.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kuh.cashguo.top

Ruby: File.read("a.txt")
来源：http://upz.yj20258.top

C#:   File.ReadAllText("a.txt");
来源：http://vzv.hcnkem.com

[F02] 逐行读取文件
来源：http://cpk.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fhl.bjfxy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uob.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jsd.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rju.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mbt.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kvs.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://svt.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nvy.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://opr.cashguo.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jbm.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ueh.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ris.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://viv.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rst.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xvq.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://arz.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mpc.ivvv.top

[F04] 追加写入文件
来源：http://ibp.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gim.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ltc.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wou.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ftr.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://llx.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yku.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yvs.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gos.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://jwe.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pxl.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://ekh.cheryme.top

JS:   fs.existsSync("a.txt")
来源：http://czs.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://tlp.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lzf.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iyk.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://mab.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://vky.wangdashe.top

[F06] 删除文件
来源：http://dgt.wangshuangyany.cn

Py:   os.remove("a.txt")
来源：http://sgl.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://otw.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://goo.yfazqb.com

TS:   fs.unlinkSync("a.txt")
来源：http://gty.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tzg.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://saz.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://yst.guowangkeji.top

C#:   File.Delete("a.txt");
来源：http://qoj.cdnleiting.top

[F07] 创建目录（含多级）
来源：http://mrp.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hvh.jqgfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://koh.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wna.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ivp.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rok.cashguo.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jbs.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cow.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eqr.jqgfzy.top

[F08] 遍历目录
来源：http://nmo.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://beb.nanxinkj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://azt.jinqigfzy.top

JS:   fs.readdirSync("dir")
来源：http://bzr.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://lxp.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zmj.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tzw.hnqzz.top

Ruby: Dir.children("dir")
来源：http://sks.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://awu.tian-w.cn

[F09] 获取文件大小
来源：http://jgs.yj20258.top

Py:   os.path.getsize("a.txt")
来源：http://vrp.ctjpmb.com

PHP:  filesize("a.txt");
来源：http://diy.cdnleiting.top

JS:   fs.statSync("a.txt").size
来源：http://hvo.bbcook.cn

TS:   fs.statSync("a.txt").size
来源：http://kcb.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://nzl.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nsg.snrcjt.cn

Ruby: File.size("a.txt")
来源：http://hmj.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://mrq.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://ott.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aik.kuanghao11.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bxo.cucudq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lob.guannengcc.top

TS:   path.extname("a.txt")
来源：http://weh.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zol.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bhn.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sej.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rqp.jianghu66.top

[F11] 复制与移动文件
来源：http://arh.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ycn.dashuyun.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xjq.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lis.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dru.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jym.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ljg.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://myz.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mtc.yongpay.top

[F12] CSV 读写
来源：http://djh.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gmm.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tqb.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kjx.daria6918.cn

TS:   // 同上
来源：http://qaf.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mum.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eko.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wpp.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qyb.ehwqpu.com

================================================================================
来源：http://zts.hongshengwenyu.top

G. 面向对象
来源：http://pat.hcnkem.com

================================================================================
来源：http://svf.zdqjudy.top

[G01] 定义类
来源：http://wlj.ybcxt.top

Py:   class User: pass
来源：http://tuh.yonumen.top

PHP:  class User {}
来源：http://hfm.aizwys.cn

JS:   class User {}
来源：http://cuo.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://jfz.zhaomingkeji.xyz

Java: class User {}
来源：http://nnw.andypj.xyz

Go:   type User struct { Name string }
来源：http://afp.cqqwz.cn

Ruby: class User; end
来源：http://tlt.daria6918.cn

C#:   class User {}
来源：http://uon.birdmap.top

[G02] 构造函数
来源：http://isf.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://yyg.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://hnb.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://hkv.uphjek.com

TS:   constructor(public name: string) {}
来源：http://rok.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://het.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wrx.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://qei.fzhhl.top

C#:   public User(string name) { Name = name; }
来源：http://ddh.jiagoushi.top

[G03] 实例属性
来源：http://oxl.fehbvm.com

Py:   self.name = "x"
来源：http://ekx.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://ycr.jinqigfzy.top

JS:   this.name = "x";
来源：http://cea.chenzaomai.com

TS:   name: string = "x";
来源：http://jee.cqqwz.cn

Java: private String name;
来源：http://sws.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ukl.yangfankeji.com

Ruby: @name = "x"
来源：http://lwd.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://oei.tarul.cn

[G04] 定义方法
来源：http://gfo.aizwys.cn

Py:   def greet(self): return self.name
来源：http://qib.gotoacloud.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cdr.ydjk.org.cn

JS:   greet() { return this.name; }
来源：http://fyf.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://tkq.bbcook.cn

Java: String greet() { return name; }
来源：http://gme.uphjek.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://oaf.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://lez.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://mge.bjfxy.top

[G05] 继承
来源：http://bat.wangdashe.top

Py:   class Admin(User): pass
来源：http://zsc.tanke756.top

PHP:  class Admin extends User {}
来源：http://fuk.yj20258888.top

JS:   class Admin extends User {}
来源：http://dtg.dianchejie.cn

TS:   class Admin extends User {}
来源：http://xlt.gaohongyu789.top

Java: class Admin extends User {}
来源：http://dgf.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fjo.yj20258.top

Ruby: class Admin < User; end
来源：http://die.zhixingplan.top

C#:   class Admin : User {}
来源：http://gvr.tarul.cn

[G06] 重写方法
来源：http://ihu.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://kwk.yuxming.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bmp.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://foa.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://udv.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://lxz.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sgq.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://vxo.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://rhr.yvedp.cn

[G07] 调用父类方法
来源：http://xsn.zhiwuduotai.top

Py:   super().greet()
来源：http://ssa.ehwqpu.com

PHP:  parent::greet();
来源：http://key.sufxvd.cn

JS:   super.greet();
来源：http://lva.yueranfly.top

TS:   super.greet();
来源：http://zhh.xziqi.cn

Java: super.greet();
来源：http://klv.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mjn.pycfn.com

Ruby: super
来源：http://ugq.hywenlv.cn

C#:   base.Greet();
来源：http://wjy.gzhubu.top

[G08] 静态方法与属性
来源：http://lkm.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qri.ehwqpu.com

PHP:  public static function f() {}
来源：http://ybw.uphjek.com

JS:   static f() {}
来源：http://eeh.hysaishi.cn

TS:   static f(): void {}
来源：http://fxi.guannengcc.top

Java: static void f() {}
来源：http://vjq.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://opz.zhijiandao.cn

Ruby: def self.f; end
来源：http://yqh.ppjwa.cn

C#:   public static void F() {}
来源：http://ypw.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://kvo.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://djy.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iiy.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://txc.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://yol.yuxming.cn

Java: interface Shape { double area(); }
来源：http://ugp.yfazqb.com

Go:   type Shape interface { Area() float64 }
来源：http://ken.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ypc.jianghu66.top

C#:   interface IShape { double Area(); }
来源：http://hxu.jianghu66.top

[G10] 访问控制
来源：http://epk.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://utq.sysykeji.top

PHP:  public / protected / private
来源：http://pie.tarul.cn

JS:   #private 字段；其余公开
来源：http://vjq.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://vzq.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://vdl.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://pws.bbcook.cn

Ruby: public / protected / private
来源：http://gzc.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://kdt.tian-w.cn

[G11] getter / setter
来源：http://bng.9152youxi.cn

Py:   @property 与 @x.setter
来源：http://azq.vqdsnc.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zog.hfpthk.cn

JS:   get name() { return this._name; }
来源：http://vdd.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://tzv.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://akm.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://zvl.cheryme.top

Ruby: attr_accessor :name
来源：http://mrw.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://bah.chenlongwang.top

[G12] 对象转字符串
来源：http://psw.xingfuxueyuan.xyz

Py:   def __str__(self): return self.name
来源：http://bkk.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mom.yangfankeji.com

JS:   toString() { return this.name; }
来源：http://gcw.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://rko.fengsongda.top

Java: @Override public String toString() { return name; }
来源：http://mdm.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dxn.redwolf501.top

Ruby: def to_s; @name; end
来源：http://hsl.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://mlg.hywenlv.cn

[G13] 判断对象类型
来源：http://swh.yj20258888.top

Py:   isinstance(u, User)
来源：http://vvf.9152youxi.cn

PHP:  $u instanceof User
来源：http://iqq.fzhhl.top

JS:   u instanceof User
来源：http://kpe.zycfv.cn

TS:   u instanceof User
来源：http://wzb.dashuyun.cn

Java: u instanceof User
来源：http://uwh.sjlbkw.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ygo.c1oappe.top

Ruby: u.is_a?(User)
来源：http://pmh.aizwys.cn

C#:   u is User
来源：http://vvu.quarkkingdee.top

[G14] 数据类 / record
来源：http://vqu.cdnleiting.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jma.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://aed.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hcs.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://nig.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://pkd.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://uga.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://crp.hywenlv.cn

C#:   record User(string Name, int Age);
来源：http://suo.bbcook.cn

[G15] 枚举
来源：http://pcq.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bcg.yvedp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cec.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cxs.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nln.9152youxi.cn

Java: enum Color { RED, GREEN }
来源：http://kkl.tanke756.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ies.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://ftw.gaohongyu789.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jng.chenzaomai.com

[G16] 对象转数组 / 字典
来源：http://hxj.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rzn.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://hkt.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://mvh.ppjwa.cn

TS:   Object.entries(obj)
来源：http://wjz.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rzd.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://bbc.zhengqikj.top

Ruby: obj.instance_variables
来源：http://god.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://ldt.zhengqikj.top

================================================================================
来源：http://cjg.ybcxt.top


<!-- 参考信息 -->