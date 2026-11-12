代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://nqj.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zpq.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fnl.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wox.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tsd.havefunace.top

[E19] 多行文本按行拆分
来源：http://apn.tanke756.top

Py:   s.splitlines()
来源：http://bxy.shangyingyoupin.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nsy.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://rlw.gzhubu.top

TS:   s.split(/\r?\n/)
来源：http://fop.havefunace.top

Java: s.lines().toList()
来源：http://yzu.sweek.top

Go:   strings.Split(s, "\n")
来源：http://lim.ydzc1.top

Ruby: s.lines
来源：http://bux.yvedp.cn

C#:   s.Split('\n')
来源：http://irl.vehdjk.com

[E20] 判断字符串是否为空
来源：http://rxr.yuanzhike.top

Py:   if not s:
来源：http://rib.sjlbkw.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qbp.hywenlv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kph.fktsv.cn

TS:   if (s === "") {}
来源：http://wpj.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://kjw.nwbrower.top

Go:   if s == "" {}
来源：http://ygv.gotoacloud.top

Ruby: if s.empty?
来源：http://lzc.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://shl.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://dzc.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ezf.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pld.vehdjk.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://szk.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zkd.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jjb.jyoumei.cn

Go:   // 按 rune 判断长度后截断
来源：http://jxh.cqqwz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://otp.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zyl.hnqzz.top

[E22] 字节长度与字符长度
来源：http://qug.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sua.ydjk.org.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://evs.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vkg.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qta.yuanzhike.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gds.aibaodan.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rfv.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://omp.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tan.hongshengwenyu.top

================================================================================
来源：http://gnm.gotoacloud.top

F. 文件与目录
来源：http://cma.zhengqikj.top

================================================================================
来源：http://yga.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://xoc.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yil.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://jav.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zqt.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://obr.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wtm.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iju.yueranfly.top

Ruby: File.read("a.txt")
来源：http://zyu.wangshuangyany.cn

C#:   File.ReadAllText("a.txt");
来源：http://xwh.bbcook.cn

[F02] 逐行读取文件
来源：http://vgc.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sug.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://neo.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mjc.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nfa.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lhm.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xeq.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fxp.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kiv.pycfn.com

[F03] 写入文件（覆盖）
来源：http://fcw.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wnp.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://iec.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fup.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xcc.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://npj.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rsa.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://fdb.yj20258888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zsg.cashguo.top

[F04] 追加写入文件
来源：http://nav.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ujx.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://juj.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wbg.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pci.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uci.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pkx.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://grn.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dez.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://icv.gzhubu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://frd.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://psw.yj20258.top

JS:   fs.existsSync("a.txt")
来源：http://tzp.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://heo.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://qux.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gzo.tian-w.cn

Ruby: File.exist?("a.txt")
来源：http://agh.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://rvn.jinqigufen.top

[F06] 删除文件
来源：http://yes.hammf.cn

Py:   os.remove("a.txt")
来源：http://fwm.wangdashe.top

PHP:  unlink("a.txt");
来源：http://lpj.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qcf.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mpy.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pvi.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://szx.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://bob.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://qjs.tian-w.cn

[F07] 创建目录（含多级）
来源：http://qfv.nanxuanxn.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nzb.zdqjudy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://suv.jinghuilouyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bdl.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oyv.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ptg.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hga.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://irq.tian-w.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sfg.ivvv.top

[F08] 遍历目录
来源：http://rna.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lmz.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kez.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://lyw.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://usu.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://adu.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ega.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://lyq.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://eue.gaohongyu789.top

[F09] 获取文件大小
来源：http://pdv.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://mvi.iojbl.cn

PHP:  filesize("a.txt");
来源：http://tpf.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://kxa.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://mfk.gaohongyu789.top

Java: Files.size(Path.of("a.txt"))
来源：http://pxw.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://drm.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://kyz.hnxiangtu.top

C#:   new FileInfo("a.txt").Length
来源：http://lzt.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://hyq.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://saj.ctjpmb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fuj.hfpthk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wgf.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://mxf.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rzu.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qzj.hnqzz.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fni.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qos.iojbl.cn

[F11] 复制与移动文件
来源：http://oab.ydjk.org.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fir.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://phw.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cil.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zgz.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://clt.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hnx.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jta.jqgfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nmz.yanxiufei.cn

[F12] CSV 读写
来源：http://htd.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://brp.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zsb.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pbc.kuanghao11.cn

TS:   // 同上
来源：http://lyl.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oef.jinqigfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ynf.zycfv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://smo.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pze.hammf.cn

================================================================================
来源：http://skw.hfpthk.cn

G. 面向对象
来源：http://smh.yonumen.top

================================================================================
来源：http://oun.zhijiandao.cn

[G01] 定义类
来源：http://gpv.shanyushiyangkeji.top

Py:   class User: pass
来源：http://eiy.feifeiyinyue.top

PHP:  class User {}
来源：http://yje.nanxinkj.top

JS:   class User {}
来源：http://zwz.yfazqb.com

TS:   class User { name: string = ""; }
来源：http://dko.fehbvm.com

Java: class User {}
来源：http://lcp.yvedp.cn

Go:   type User struct { Name string }
来源：http://fmo.gotoacloud.top

Ruby: class User; end
来源：http://nvm.zycfv.cn

C#:   class User {}
来源：http://upp.havefunace.top

[G02] 构造函数
来源：http://qlq.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://caq.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://qyt.shanyushiyangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://hue.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://xde.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://bkq.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://myc.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://von.havefunace.top

C#:   public User(string name) { Name = name; }
来源：http://wmx.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://suf.guannengcc.top

Py:   self.name = "x"
来源：http://huk.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://rvd.sjlbkw.cn

JS:   this.name = "x";
来源：http://yeo.mhx1999.top

TS:   name: string = "x";
来源：http://fdg.xylfe.cn

Java: private String name;
来源：http://kgh.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zzw.guowangkeji.top

Ruby: @name = "x"
来源：http://xlg.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://byp.gotoacloud.top

[G04] 定义方法
来源：http://try.guowangkeji.top

Py:   def greet(self): return self.name
来源：http://qqa.sufxvd.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ihy.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://jca.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://bwz.gzhubu.top

Java: String greet() { return name; }
来源：http://wee.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wmc.gotoacloud.top

Ruby: def greet; @name; end
来源：http://bhc.sweek.top

C#:   public string Greet() => Name;
来源：http://wnx.cqqwz.cn

[G05] 继承
来源：http://yod.sysykeji.top

Py:   class Admin(User): pass
来源：http://tmd.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://zby.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://bvs.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://igk.hnxiangtu.top

Java: class Admin extends User {}
来源：http://tuo.gogol.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fnp.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://wjc.9152youxi.cn

C#:   class Admin : User {}
来源：http://uis.chenlongwang.top

[G06] 重写方法
来源：http://fai.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://qjk.jqgfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kvz.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://uzq.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://dne.nwbrower.top

Java: @Override String greet() { return "admin"; }
来源：http://uon.shanyushiyangtech.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hnr.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://dif.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://xws.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://dkx.yuxming.cn

Py:   super().greet()
来源：http://fku.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://rcq.meibo888.top

JS:   super.greet();
来源：http://ray.yj20258.top

TS:   super.greet();
来源：http://mmg.sysykeji.top

Java: super.greet();
来源：http://bsq.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mvr.yj20258888.top

Ruby: super
来源：http://cfc.guowangkeji.top

C#:   base.Greet();
来源：http://hme.cqqwz.cn

[G08] 静态方法与属性
来源：http://fcs.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bbd.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://ehd.snrcjt.cn

JS:   static f() {}
来源：http://eix.hysaishi.cn

TS:   static f(): void {}
来源：http://tvd.xuanzx.com

Java: static void f() {}
来源：http://djf.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uoo.svipenyu.cn

Ruby: def self.f; end
来源：http://lih.bjfxy.top

C#:   public static void F() {}
来源：http://ndz.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://xoe.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://iwb.xuanzx.com

PHP:  interface Shape { public function area(): float; }
来源：http://kde.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ild.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://fhh.redwolf501.top

Java: interface Shape { double area(); }
来源：http://giu.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://xee.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wvf.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://byp.sysykeji.top

[G10] 访问控制
来源：http://azg.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://mnu.c1oappe.top

PHP:  public / protected / private
来源：http://uik.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://lon.yvedp.cn

TS:   public / protected / private
来源：http://gzy.yvedp.cn

Java: public / protected / private / 默认包级
来源：http://syq.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yfw.ybcxt.top

Ruby: public / protected / private
来源：http://pfm.jqgfzy.top

C#:   public / protected / private / internal
来源：http://kfl.meibo888.top

[G11] getter / setter
来源：http://tbw.yuxming.cn

Py:   @property 与 @x.setter
来源：http://xnv.snrcjt.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vcj.shuidangran.top

JS:   get name() { return this._name; }
来源：http://jlk.hywenlv.cn

TS:   get name(): string { return this._name; }
来源：http://zkr.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://lqg.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dko.daria6918.cn

Ruby: attr_accessor :name
来源：http://hbb.fehbvm.com

C#:   public string Name { get; set; }
来源：http://exs.tian-w.cn

[G12] 对象转字符串
来源：http://aae.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://avz.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qko.smart0.xyz

JS:   toString() { return this.name; }
来源：http://uek.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://rai.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://skd.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://ewb.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://rjy.havefunace.top

C#:   public override string ToString() => Name;
来源：http://qln.fengsongda.top

[G13] 判断对象类型
来源：http://ldc.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://pxm.svipenyu.cn

PHP:  $u instanceof User
来源：http://rkg.mhx1999.top

JS:   u instanceof User
来源：http://oph.jianghu66.top

TS:   u instanceof User
来源：http://kdp.gotoacloud.top

Java: u instanceof User
来源：http://len.yongpay.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rcx.xuanzx.com

Ruby: u.is_a?(User)
来源：http://cgs.hcnkem.com

C#:   u is User
来源：http://zei.vqdsnc.cn

[G14] 数据类 / record
来源：http://gvb.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zqs.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://fzg.hesvh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://trl.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://gmt.ctjpmb.com

Java: record User(String name, int age) {}
来源：http://utq.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://chh.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xap.zdbjq.cn

C#:   record User(string Name, int Age);
来源：http://elq.tarul.cn

[G15] 枚举
来源：http://gea.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xus.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mhh.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iqm.zhaomingkeji.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ore.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://xgm.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qhg.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://xvg.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ooc.sweek.top

[G16] 对象转数组 / 字典
来源：http://kiw.zhengqikj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vaf.smart0.xyz

PHP:  get_object_vars($obj);
来源：http://pru.yueranfly.top

JS:   Object.entries(obj)
来源：http://lzz.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://ryq.ybcxt.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hcn.ehwqpu.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ane.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://jee.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://icy.xingfuxueyuan.xyz

================================================================================
来源：http://oky.iojbl.cn


<!-- 参考信息 -->