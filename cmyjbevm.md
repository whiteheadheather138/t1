代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://wqt.feifeiyinyue.top

TS:   s.split(/\r?\n/)
来源：http://jyl.sufxvd.cn

Java: s.lines().toList()
来源：http://oqh.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://hkd.yanxiufei.cn

Ruby: s.lines
来源：http://uwg.hnxiangtu.top

C#:   s.Split('\n')
来源：http://ziz.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://twm.shanyushiyangkeji.top

Py:   if not s:
来源：http://qem.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hrt.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cny.ivvv.top

TS:   if (s === "") {}
来源：http://rxe.hcnkem.com

Java: if (s.isEmpty()) {}
来源：http://fht.yvedp.cn

Go:   if s == "" {}
来源：http://jgd.yj202588.top

Ruby: if s.empty?
来源：http://vgl.zycfv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zoq.fktsv.cn

[E21] 超长截断加省略号
来源：http://rzq.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://flz.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xcn.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iqq.shangyingyoupin.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://otw.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tqk.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://oab.guannengcc.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rhj.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gad.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://wcm.nanxuanxn.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qij.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mew.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gur.wangshuangyany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hvp.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://okr.yuxming.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xlg.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://alp.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://krz.fanxiaobao.xyz

================================================================================
来源：http://ukr.xylfe.cn

F. 文件与目录
来源：http://xpw.andypj.xyz

================================================================================
来源：http://qpi.bjfxy.top

[F01] 读取整个文件
来源：http://nic.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yzp.gogol.net.cn

PHP:  file_get_contents("a.txt");
来源：http://hiw.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ecp.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blj.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hgp.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fln.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://tig.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://akp.yueranfly.top

[F02] 逐行读取文件
来源：http://jop.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ibf.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fvl.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dvv.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oaw.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qrn.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://syf.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://skp.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bep.uphjek.com

[F03] 写入文件（覆盖）
来源：http://abe.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nqq.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ffw.yj202588.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wdl.xinyue.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pnw.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iqc.zhiwuduotai.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fwe.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://vsg.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wag.cdnleiting.top

[F04] 追加写入文件
来源：http://pfn.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yeh.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gzm.wangdashe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wkx.yuxming.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zth.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jfs.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zjb.snrcjt.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jwk.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kwn.bjfxy.top

[F05] 判断文件或目录是否存在
来源：http://hoe.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fls.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://mpx.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://keu.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://hzx.redwolf501.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fzv.fanxiaobao.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://exe.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://xfs.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://fng.tian-w.cn

[F06] 删除文件
来源：http://son.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://wwa.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://aks.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://pod.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://ysb.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://crp.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://bqe.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://arn.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://cwe.hnqzz.top

[F07] 创建目录（含多级）
来源：http://ycv.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mhr.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qfw.guowangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iob.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qcr.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pzl.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://btq.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://acp.shangyingyoupin.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ori.mhx1999.top

[F08] 遍历目录
来源：http://jre.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://glw.bjfxy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rpi.birdmap.top

JS:   fs.readdirSync("dir")
来源：http://hjq.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://gos.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://akt.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pal.jqgfzy.top

Ruby: Dir.children("dir")
来源：http://blb.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://vjn.yj202588.top

[F09] 获取文件大小
来源：http://hfk.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://wvv.mhx1999.top

PHP:  filesize("a.txt");
来源：http://ija.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://pky.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://zih.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://neh.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cgp.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://oox.hywenlv.cn

C#:   new FileInfo("a.txt").Length
来源：http://ulx.ywan-chungtsiang.top

[F10] 取文件扩展名 / 文件名
来源：http://lfr.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lbg.hammf.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yug.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yvd.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://rtn.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dgo.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qto.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iru.svipenyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rzf.ydzc1.top

[F11] 复制与移动文件
来源：http://uad.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wyv.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mdn.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mkf.jinqigfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cek.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aez.guannengcc.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aei.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hnr.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gph.zhengqikj.top

[F12] CSV 读写
来源：http://qew.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yer.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ewo.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ghe.nanxinkj.top

TS:   // 同上
来源：http://zro.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hmp.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jzp.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nsd.0kj1m.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pbk.jyoumei.cn

================================================================================
来源：http://myt.aizwys.cn

G. 面向对象
来源：http://hwx.9152youxi.cn

================================================================================
来源：http://shn.tianlin.xyz

[G01] 定义类
来源：http://saq.daxiang520.top

Py:   class User: pass
来源：http://cyg.shangyingyoupin.top

PHP:  class User {}
来源：http://rsg.ivvv.top

JS:   class User {}
来源：http://rqm.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://cmz.9152youxi.cn

Java: class User {}
来源：http://evb.yuanzhike.top

Go:   type User struct { Name string }
来源：http://wqb.gotoacloud.top

Ruby: class User; end
来源：http://wni.meibo888.top

C#:   class User {}
来源：http://gbi.smart0.xyz

[G02] 构造函数
来源：http://wll.hysaishi.cn

Py:   def __init__(self, name): self.name = name
来源：http://ybl.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://yqv.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://dpa.hcnkem.com

TS:   constructor(public name: string) {}
来源：http://cuu.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://vlj.feifeiyinyue.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mxt.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://ffv.wangdashe.top

C#:   public User(string name) { Name = name; }
来源：http://gwf.c1oappe.top

[G03] 实例属性
来源：http://fua.bbcook.cn

Py:   self.name = "x"
来源：http://pqd.chenzaomai.com

PHP:  public string $name = "x";
来源：http://bhw.xziqi.cn

JS:   this.name = "x";
来源：http://mot.chenlongwang.top

TS:   name: string = "x";
来源：http://znf.xuetiantiany.cn

Java: private String name;
来源：http://iwo.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bdb.yvedp.cn

Ruby: @name = "x"
来源：http://lcd.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://jbk.dashuyun.cn

[G04] 定义方法
来源：http://sds.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://frm.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://aum.ivvv.top

JS:   greet() { return this.name; }
来源：http://fnw.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://iok.zhengqikj.top

Java: String greet() { return name; }
来源：http://yjl.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://geh.gzhubu.top

Ruby: def greet; @name; end
来源：http://glc.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://tkt.tarul.cn

[G05] 继承
来源：http://tog.shzxlz.cn

Py:   class Admin(User): pass
来源：http://rhn.smart0.xyz

PHP:  class Admin extends User {}
来源：http://bll.hcnkem.com

JS:   class Admin extends User {}
来源：http://anu.chenlongwang.top

TS:   class Admin extends User {}
来源：http://cwy.ivvv.top

Java: class Admin extends User {}
来源：http://zsm.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eev.hysaishi.cn

Ruby: class Admin < User; end
来源：http://gee.ctjpmb.com

C#:   class Admin : User {}
来源：http://mzq.tarul.cn

[G06] 重写方法
来源：http://vlo.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://vnm.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cqi.gzhubu.top

JS:   greet() { return "admin"; }
来源：http://kwr.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://bbc.hongshengwenyu.top

Java: @Override String greet() { return "admin"; }
来源：http://hkp.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nyj.cheryme.top

Ruby: def greet; "admin"; end
来源：http://cej.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://etw.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://xhi.sjlbkw.cn

Py:   super().greet()
来源：http://utl.cashguo.top

PHP:  parent::greet();
来源：http://cto.aibaodan.cn

JS:   super.greet();
来源：http://jrg.hcnkem.com

TS:   super.greet();
来源：http://xzh.shuidangran.top

Java: super.greet();
来源：http://rrt.hcnkem.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ova.vqdsnc.cn

Ruby: super
来源：http://unz.hnqzz.top

C#:   base.Greet();
来源：http://tym.andypj.xyz

[G08] 静态方法与属性
来源：http://ken.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://emd.meibo888.top

PHP:  public static function f() {}
来源：http://aus.zhongyouzk.top

JS:   static f() {}
来源：http://pya.yj20258888.top

TS:   static f(): void {}
来源：http://xts.hammf.cn

Java: static void f() {}
来源：http://fwz.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ads.jianghu66.top

Ruby: def self.f; end
来源：http://vkx.wangshuangyany.cn

C#:   public static void F() {}
来源：http://pwn.wangshuangyany.cn

[G09] 接口 / 抽象类
来源：http://eye.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://yvy.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://wtv.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://iiw.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://may.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://ekz.yuxming.cn

Go:   type Shape interface { Area() float64 }
来源：http://ekq.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://izb.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://fgd.gotoacloud.top

[G10] 访问控制
来源：http://uue.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://sal.haohaochexian.top

PHP:  public / protected / private
来源：http://gye.jianghu66.top

JS:   #private 字段；其余公开
来源：http://kif.tarul.cn

TS:   public / protected / private
来源：http://rdn.zhaomingkeji.xyz

Java: public / protected / private / 默认包级
来源：http://nwr.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mmd.fengsongda.top

Ruby: public / protected / private
来源：http://wxu.ydzc1.top

C#:   public / protected / private / internal
来源：http://jzn.jianghu66.top

[G11] getter / setter
来源：http://iwh.nanxuanxn.top

Py:   @property 与 @x.setter
来源：http://tbe.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mri.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://mbz.shangyingyoupin.top

TS:   get name(): string { return this._name; }
来源：http://pah.daxiang520.top

Java: public String getName() { return name; }
来源：http://lab.cqqwz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rod.chenlongwang.top

Ruby: attr_accessor :name
来源：http://fok.shuidangran.top

C#:   public string Name { get; set; }
来源：http://itq.yueranfly.top

[G12] 对象转字符串
来源：http://euj.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://dcb.hongshengwenyu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://swc.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://qff.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://rum.yfazqb.com

Java: @Override public String toString() { return name; }
来源：http://reg.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tfo.xziqi.cn

Ruby: def to_s; @name; end
来源：http://vur.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://gnc.daxiang520.top

[G13] 判断对象类型
来源：http://lmv.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://dvj.xinyue.icu

PHP:  $u instanceof User
来源：http://obs.sjlbkw.cn

JS:   u instanceof User
来源：http://klv.fengsongda.top

TS:   u instanceof User
来源：http://xpx.mhx1999.top

Java: u instanceof User
来源：http://dnp.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bri.tarul.cn

Ruby: u.is_a?(User)
来源：http://avf.fehbvm.com

C#:   u is User
来源：http://yxw.uphjek.com

[G14] 数据类 / record
来源：http://eoi.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gnk.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://czz.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://ceh.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://jyw.uphjek.com

Java: record User(String name, int age) {}
来源：http://lpx.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://sff.shzxlz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tnu.yangfankeji.com

C#:   record User(string Name, int Age);
来源：http://dqo.ydjk.org.cn

[G15] 枚举
来源：http://hja.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iwb.tanke756.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vwc.cucudq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vsl.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rtr.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://biy.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bfc.jiagoushi.top

Ruby: Color = %i[red green].freeze
来源：http://wmz.jqgufenzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://juf.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://tzn.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rxe.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://zbz.nwbrower.top

JS:   Object.entries(obj)
来源：http://pwh.meibo888.top

TS:   Object.entries(obj)
来源：http://ela.ywan-chungtsiang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jch.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gux.c1oappe.top

Ruby: obj.instance_variables
来源：http://sza.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://rie.cdnleiting.top

================================================================================
来源：http://zwy.snrcjt.cn

H. 异常与错误处理
来源：http://upt.hcnkem.com

================================================================================
来源：http://ohz.yanxiufei.cn

[H01] try / catch 基础
来源：http://uck.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ubt.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eau.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zhz.havefunace.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://djz.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zee.bjfxy.top


<!-- 参考信息 -->