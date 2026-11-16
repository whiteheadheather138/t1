代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ytn.gzhubu.top

[E19] 多行文本按行拆分
来源：http://umc.guowangkeji.top

Py:   s.splitlines()
来源：http://opg.cashguo.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ycx.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://qka.ydjk.org.cn

TS:   s.split(/\r?\n/)
来源：http://lpt.jinqigfzy.top

Java: s.lines().toList()
来源：http://iqe.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://srw.hywenlv.cn

Ruby: s.lines
来源：http://gey.zdbjq.cn

C#:   s.Split('\n')
来源：http://ghq.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://kod.52xcode.cn

Py:   if not s:
来源：http://pri.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zxn.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://knm.bbcook.cn

TS:   if (s === "") {}
来源：http://rpi.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://vlq.zdqjudy.top

Go:   if s == "" {}
来源：http://yoy.cdnleiting.top

Ruby: if s.empty?
来源：http://wcc.ydzc1.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uxp.c1oappe.top

[E21] 超长截断加省略号
来源：http://ppz.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://snr.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lcy.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ghz.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kjs.yangfankeji.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ahw.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://wcu.yuxming.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yzd.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oke.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://yfk.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://juk.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://akr.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cmt.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dhd.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uqu.hammf.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://srs.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://leo.ehwqpu.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jig.daria6918.cn

================================================================================
来源：http://vyk.xziqi.cn

F. 文件与目录
来源：http://jnd.wangshuangyany.cn

================================================================================
来源：http://eca.fzhhl.top

[F01] 读取整个文件
来源：http://rgc.cashguo.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dmz.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://duc.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xvi.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ydg.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xlh.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ail.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://jgf.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://czb.wangdashe.top

[F02] 逐行读取文件
来源：http://kgi.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jlc.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hei.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dbf.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rrw.smart0.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ael.feifeiyinyue.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cwm.vqdsnc.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xmx.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bdo.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://ivu.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xsm.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://syn.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dbw.hysaishi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ewo.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qbv.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://alh.xziqi.cn

Ruby: File.write("a.txt", "hi")
来源：http://oab.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://swq.xziqi.cn

[F04] 追加写入文件
来源：http://zas.hongshengwenyu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lju.sxryk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bga.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xtx.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mdq.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ogm.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pok.yuanzhike.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xwz.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ybu.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://ver.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ces.zhixingplan.top

PHP:  file_exists("a.txt");
来源：http://sgo.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://ish.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://wrc.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jrd.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://idt.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://ibv.yj20258888.top

C#:   File.Exists("a.txt")
来源：http://oic.hesvh.cn

[F06] 删除文件
来源：http://lqt.bjfxy.top

Py:   os.remove("a.txt")
来源：http://rsx.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://qgh.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mtv.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://tjy.nwbrower.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ldd.cashguo.top

Go:   os.Remove("a.txt")
来源：http://cfk.gzhubu.top

Ruby: File.delete("a.txt")
来源：http://dga.nanxuanxn.top

C#:   File.Delete("a.txt");
来源：http://kmj.tian-w.cn

[F07] 创建目录（含多级）
来源：http://jco.svipenyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lga.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://osn.daria6918.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zed.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yic.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jdr.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ekt.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cto.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uwp.yongpay.top

[F08] 遍历目录
来源：http://ymu.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://aiz.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kfs.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://vnv.gaohongyu789.top

TS:   fs.readdirSync("dir")
来源：http://lny.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fjv.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dfd.andypj.xyz

Ruby: Dir.children("dir")
来源：http://tec.redwolf501.top

C#:   Directory.GetFiles("dir")
来源：http://rvw.chenjidiqi.icu

[F09] 获取文件大小
来源：http://rdu.yueranfly.top

Py:   os.path.getsize("a.txt")
来源：http://ecz.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://kao.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://adw.cashguo.top

TS:   fs.statSync("a.txt").size
来源：http://ima.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://myx.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jtx.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://xlq.nanxuanxn.top

C#:   new FileInfo("a.txt").Length
来源：http://itb.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://pfm.tanke756.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pas.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jun.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uty.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://lct.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cho.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zny.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ili.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rsa.hesvh.cn

[F11] 复制与移动文件
来源：http://oan.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lat.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://exc.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cmb.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ajz.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://low.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vrx.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rcx.wangshuangyany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bqf.yuanzhike.top

[F12] CSV 读写
来源：http://dqw.cucudq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fhf.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jds.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vbc.yfazqb.com

TS:   // 同上
来源：http://lum.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mob.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qng.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tny.zhengqikj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ovg.smart0.xyz

================================================================================
来源：http://khg.hesvh.cn

G. 面向对象
来源：http://xlm.andypj.xyz

================================================================================
来源：http://xfk.yueranfly.top

[G01] 定义类
来源：http://jat.tanke756.top

Py:   class User: pass
来源：http://lmb.chenzaomai.com

PHP:  class User {}
来源：http://kei.hfpthk.cn

JS:   class User {}
来源：http://erh.gaohongyu789.top

TS:   class User { name: string = ""; }
来源：http://mqx.jinyuanbaomall.cn

Java: class User {}
来源：http://nuq.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://hbk.fengsongda.top

Ruby: class User; end
来源：http://box.zycfv.cn

C#:   class User {}
来源：http://dba.zhiwuduotai.top

[G02] 构造函数
来源：http://mlh.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://xcb.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://bnx.xinyue.icu

JS:   constructor(name) { this.name = name; }
来源：http://dvv.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://ytf.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://zyv.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ipj.gotoacloud.top

Ruby: def initialize(name); @name = name; end
来源：http://lfs.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://wdp.fengsongda.top

[G03] 实例属性
来源：http://scv.guannengcc.top

Py:   self.name = "x"
来源：http://ptr.hcnkem.com

PHP:  public string $name = "x";
来源：http://afg.gogol.net.cn

JS:   this.name = "x";
来源：http://svf.epnwcf.com

TS:   name: string = "x";
来源：http://jow.smart0.xyz

Java: private String name;
来源：http://ihk.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bpu.jlsjyb.cn

Ruby: @name = "x"
来源：http://ywr.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://ljb.aibaodan.cn

[G04] 定义方法
来源：http://ycx.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://tzg.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rmz.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://oay.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://qax.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://vvk.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mij.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://wek.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://zot.cqqwz.cn

[G05] 继承
来源：http://bqa.yangfankeji.com

Py:   class Admin(User): pass
来源：http://dag.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://ube.c1oappe.top

JS:   class Admin extends User {}
来源：http://xkk.yueranfly.top

TS:   class Admin extends User {}
来源：http://hfl.haohaochexian.top

Java: class Admin extends User {}
来源：http://yqw.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vqo.hcnkem.com

Ruby: class Admin < User; end
来源：http://kvv.pycfn.com

C#:   class Admin : User {}
来源：http://ipw.nwbrower.top

[G06] 重写方法
来源：http://xcc.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://swp.jqgfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bkx.yj20258.top

JS:   greet() { return "admin"; }
来源：http://bxx.havefunace.top

TS:   greet(): string { return "admin"; }
来源：http://atj.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://xgx.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ket.yfazqb.com

Ruby: def greet; "admin"; end
来源：http://rss.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://ses.xylfe.cn

[G07] 调用父类方法
来源：http://wsd.vqdsnc.cn

Py:   super().greet()
来源：http://dut.svipenyu.cn

PHP:  parent::greet();
来源：http://lvi.zhiwuduotai.top

JS:   super.greet();
来源：http://jzj.fanxiaobao.xyz

TS:   super.greet();
来源：http://fzb.sweek.top

Java: super.greet();
来源：http://kyx.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gzt.fehbvm.com

Ruby: super
来源：http://gki.hysaishi.cn

C#:   base.Greet();
来源：http://rfd.zdbjq.cn

[G08] 静态方法与属性
来源：http://aln.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ild.xinyue.icu

PHP:  public static function f() {}
来源：http://wxv.chenlongwang.top

JS:   static f() {}
来源：http://fow.cdnleiting.top

TS:   static f(): void {}
来源：http://bau.yuxming.cn

Java: static void f() {}
来源：http://qof.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vzn.fehbvm.com

Ruby: def self.f; end
来源：http://vni.sufxvd.cn

C#:   public static void F() {}
来源：http://duk.xuanzx.com

[G09] 接口 / 抽象类
来源：http://dhq.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://dst.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://ypt.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ajh.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://xly.xuanzx.com

Java: interface Shape { double area(); }
来源：http://way.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://mvw.daria6918.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zcl.ydzc1.top

C#:   interface IShape { double Area(); }
来源：http://wix.shangyingyoupin.top

[G10] 访问控制
来源：http://juw.xziqi.cn

Py:   约定 _protected / __private（不强制）
来源：http://uqj.chenlongwang.top

PHP:  public / protected / private
来源：http://rbo.daria6918.cn

JS:   #private 字段；其余公开
来源：http://pqu.cqqwz.cn

TS:   public / protected / private
来源：http://zop.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://rwy.mhx1999.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hou.gzhubu.top

Ruby: public / protected / private
来源：http://xtk.haohaochexian.top

C#:   public / protected / private / internal
来源：http://ozd.52xcode.cn

[G11] getter / setter
来源：http://osg.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://haw.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bsa.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://ueh.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://qte.cucudq.cn

Java: public String getName() { return name; }
来源：http://nqh.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://rhz.tian-w.cn

Ruby: attr_accessor :name
来源：http://hax.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://wwn.bjfxy.top

[G12] 对象转字符串
来源：http://ppl.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://sql.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bxw.316326.xyz

JS:   toString() { return this.name; }
来源：http://sqx.zhixingplan.top

TS:   toString(): string { return this.name; }
来源：http://rqd.zhongyouzk.top

Java: @Override public String toString() { return name; }
来源：http://uth.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://xlm.uphjek.com

Ruby: def to_s; @name; end
来源：http://mwa.ydjk.org.cn

C#:   public override string ToString() => Name;
来源：http://dkr.9152youxi.cn

[G13] 判断对象类型
来源：http://xdl.bbcook.cn

Py:   isinstance(u, User)
来源：http://yow.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://fwf.daxiang520.top

JS:   u instanceof User
来源：http://lve.redwolf501.top

TS:   u instanceof User
来源：http://dpw.jyoumei.cn

Java: u instanceof User
来源：http://xdn.ywan-chungtsiang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iwz.vqdsnc.cn

Ruby: u.is_a?(User)
来源：http://hbp.yj20258888.top

C#:   u is User
来源：http://vvt.cucudq.cn

[G14] 数据类 / record
来源：http://bxk.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qzx.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://cvw.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vuv.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://oyk.gzhubu.top

Java: record User(String name, int age) {}
来源：http://qpf.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://mos.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yap.havefunace.top

C#:   record User(string Name, int Age);
来源：http://rsf.daxiang520.top

[G15] 枚举
来源：http://dcr.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tiz.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://oax.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ris.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rxs.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://ppi.yuxming.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kdr.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://qko.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fus.yonumen.top

[G16] 对象转数组 / 字典
来源：http://avy.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bwv.zhixingplan.top

PHP:  get_object_vars($obj);
来源：http://yyf.yongpay.top

JS:   Object.entries(obj)
来源：http://lac.hfpthk.cn

TS:   Object.entries(obj)
来源：http://mma.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uux.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iqu.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://ktu.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://dsg.redwolf501.top

================================================================================
来源：http://xxn.fanxiaobao.xyz

H. 异常与错误处理
来源：http://jfl.ppjwa.cn

================================================================================
来源：http://tii.guowangkeji.top

[H01] try / catch 基础
来源：http://qyn.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ixw.nanxuanxn.top


<!-- 参考信息 -->