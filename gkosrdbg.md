代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kwc.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://bnf.yanxiufei.cn

Py:   s.splitlines()
来源：http://bii.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hek.sjlbkw.cn

JS:   s.split(/\r?\n/)
来源：http://let.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://fyl.ehwqpu.com

Java: s.lines().toList()
来源：http://uwc.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://dgz.kuanghao11.cn

Ruby: s.lines
来源：http://amc.mhx1999.top

C#:   s.Split('\n')
来源：http://epd.ppjwa.cn

[E20] 判断字符串是否为空
来源：http://cvn.hesvh.cn

Py:   if not s:
来源：http://vga.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ynf.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bgi.jqgfzy.top

TS:   if (s === "") {}
来源：http://yes.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://iem.aizwys.cn

Go:   if s == "" {}
来源：http://wfr.yangfankeji.com

Ruby: if s.empty?
来源：http://chc.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wzm.zhixingplan.top

[E21] 超长截断加省略号
来源：http://ktn.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://erf.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ele.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://obp.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mjb.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zgx.aizwys.cn

Go:   // 按 rune 判断长度后截断
来源：http://fop.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://atx.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gdt.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://dym.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aoj.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wvo.vqdsnc.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://icw.dianchejie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rok.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qml.nanxinkj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tqv.nanxuanxn.top

Ruby: s.bytesize;  s.length
来源：http://ifc.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jlo.aizwys.cn

================================================================================
来源：http://kds.vqdsnc.cn

F. 文件与目录
来源：http://ixh.jianghu66.top

================================================================================
来源：http://ubc.nanxinkj.top

[F01] 读取整个文件
来源：http://otf.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cim.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://oyj.zhaomingkeji.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://usq.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xir.birdmap.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yle.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lso.zycfv.cn

Ruby: File.read("a.txt")
来源：http://nzh.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://ooj.zhijiandao.cn

[F02] 逐行读取文件
来源：http://fsc.hnqzz.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gtx.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xrj.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ldn.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kip.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qhm.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vjf.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rnz.ctjpmb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cxi.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://bso.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tcx.jqgufenzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vtq.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pdn.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fif.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mbb.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dbq.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://bbp.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://osl.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://eeh.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tne.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ouy.jianghu66.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fmt.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://myx.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ycr.fengsongda.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ayu.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://njm.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sgj.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://jye.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uth.hcnkem.com

PHP:  file_exists("a.txt");
来源：http://kor.sufxvd.cn

JS:   fs.existsSync("a.txt")
来源：http://dud.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://dtx.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://gvf.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hcu.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://yjw.havefunace.top

C#:   File.Exists("a.txt")
来源：http://bwy.sysykeji.top

[F06] 删除文件
来源：http://asr.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://pla.tanke756.top

PHP:  unlink("a.txt");
来源：http://qga.uphjek.com

JS:   fs.unlinkSync("a.txt")
来源：http://lji.sxryk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://asr.yj20258888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zya.pengpengdd.cyou

Go:   os.Remove("a.txt")
来源：http://suq.yj20258.top

Ruby: File.delete("a.txt")
来源：http://mvs.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://cfh.zycfv.cn

[F07] 创建目录（含多级）
来源：http://joe.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qda.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hzf.ctjpmb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mth.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pwd.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zjb.jinghuilouyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qph.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cvb.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wdz.andypj.xyz

[F08] 遍历目录
来源：http://sgg.zycfv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bzr.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qzk.jinyuanbaomall.cn

JS:   fs.readdirSync("dir")
来源：http://miq.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://wqs.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rjv.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xhi.guannengcc.top

Ruby: Dir.children("dir")
来源：http://saj.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://zcc.tanke756.top

[F09] 获取文件大小
来源：http://jpm.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://glj.yonumen.top

PHP:  filesize("a.txt");
来源：http://wzz.cqqwz.cn

JS:   fs.statSync("a.txt").size
来源：http://wej.sweek.top

TS:   fs.statSync("a.txt").size
来源：http://jon.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fae.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rmv.yongpay.top

Ruby: File.size("a.txt")
来源：http://qvv.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://xnl.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://zox.shzxlz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jpj.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wxy.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mvm.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://vln.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wru.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://muw.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bzv.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pri.yanxiufei.cn

[F11] 复制与移动文件
来源：http://nut.sxryk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://huk.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://upb.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xbr.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lte.gzhubu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ovq.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uhn.ctjpmb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wyx.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ltp.nwbrower.top

[F12] CSV 读写
来源：http://ebc.tanke756.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qiq.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fji.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rwi.zdbjq.cn

TS:   // 同上
来源：http://bmw.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ljs.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wcy.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sqx.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://mnr.sweek.top

================================================================================
来源：http://tic.bjfxy.top

G. 面向对象
来源：http://ehb.yuanzhike.top

================================================================================
来源：http://wdt.yongpay.top

[G01] 定义类
来源：http://dln.sxryk.cn

Py:   class User: pass
来源：http://urr.zhongyouzk.top

PHP:  class User {}
来源：http://ucp.cqqwz.cn

JS:   class User {}
来源：http://imn.gzhubu.top

TS:   class User { name: string = ""; }
来源：http://bzf.yj20258888.top

Java: class User {}
来源：http://cir.ivvv.top

Go:   type User struct { Name string }
来源：http://oxh.tanke756.top

Ruby: class User; end
来源：http://iiu.dashuyun.cn

C#:   class User {}
来源：http://diy.xuanzx.com

[G02] 构造函数
来源：http://sle.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://yrc.jyoumei.cn

PHP:  public function __construct(public string $name) {}
来源：http://vhq.chenlongwang.top

JS:   constructor(name) { this.name = name; }
来源：http://bqr.yj20258.top

TS:   constructor(public name: string) {}
来源：http://emj.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://uvu.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vdj.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://ftc.quarkkingdee.top

C#:   public User(string name) { Name = name; }
来源：http://wqg.wangshuangyany.cn

[G03] 实例属性
来源：http://xkh.meibo888.top

Py:   self.name = "x"
来源：http://fmz.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://esl.zhijiandao.cn

JS:   this.name = "x";
来源：http://xww.xinyue.icu

TS:   name: string = "x";
来源：http://osz.gaohongyu789.top

Java: private String name;
来源：http://ltg.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wnx.ydjk.org.cn

Ruby: @name = "x"
来源：http://puu.hcnkem.com

C#:   public string Name { get; set; } = "x";
来源：http://alh.chenlongwang.top

[G04] 定义方法
来源：http://vqh.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://ssj.cqqwz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bxt.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://bnp.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://zyc.sjlbkw.cn

Java: String greet() { return name; }
来源：http://vwf.xuanzx.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://tcy.cqqwz.cn

Ruby: def greet; @name; end
来源：http://cej.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://kbi.9152youxi.cn

[G05] 继承
来源：http://hjh.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://ywk.pycfn.com

PHP:  class Admin extends User {}
来源：http://bdj.feifeiyinyue.top

JS:   class Admin extends User {}
来源：http://osb.hysaishi.cn

TS:   class Admin extends User {}
来源：http://foy.xuanzx.com

Java: class Admin extends User {}
来源：http://ras.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ydi.hnxiangtu.top

Ruby: class Admin < User; end
来源：http://grd.feifeiyinyue.top

C#:   class Admin : User {}
来源：http://njn.guannengcc.top

[G06] 重写方法
来源：http://ykc.jlsjyb.cn

Py:   def greet(self): return "admin"
来源：http://mpm.zdqjudy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zem.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://rhj.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://lyt.bbcook.cn

Java: @Override String greet() { return "admin"; }
来源：http://mzr.cucudq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vfi.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://ybc.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://oge.zhixingplan.top

[G07] 调用父类方法
来源：http://icn.yj202588.top

Py:   super().greet()
来源：http://fax.jqgfzy.top

PHP:  parent::greet();
来源：http://aod.yvedp.cn

JS:   super.greet();
来源：http://voa.zhoulong.xyz

TS:   super.greet();
来源：http://gds.daxiang520.top

Java: super.greet();
来源：http://wxd.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://agb.xziqi.cn

Ruby: super
来源：http://jie.ydjk.org.cn

C#:   base.Greet();
来源：http://suk.bjfxy.top

[G08] 静态方法与属性
来源：http://eee.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lsr.cheryme.top

PHP:  public static function f() {}
来源：http://vez.xziqi.cn

JS:   static f() {}
来源：http://jlx.zhijiandao.cn

TS:   static f(): void {}
来源：http://qrg.zhoulong.xyz

Java: static void f() {}
来源：http://yua.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hvq.yonumen.top

Ruby: def self.f; end
来源：http://gmn.ctjpmb.com

C#:   public static void F() {}
来源：http://lij.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://eef.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://zzo.jinyuanbaomall.cn

PHP:  interface Shape { public function area(): float; }
来源：http://phx.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://ecq.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://hba.tanke756.top

Java: interface Shape { double area(); }
来源：http://nui.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://aty.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://unm.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://don.snrcjt.cn

[G10] 访问控制
来源：http://zjj.zhengqikj.top

Py:   约定 _protected / __private（不强制）
来源：http://zff.guowangkeji.top

PHP:  public / protected / private
来源：http://ynx.yueranfly.top

JS:   #private 字段；其余公开
来源：http://khv.yueranfly.top

TS:   public / protected / private
来源：http://yol.zhixingplan.top

Java: public / protected / private / 默认包级
来源：http://esi.vqdsnc.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gdr.jlsjyb.cn

Ruby: public / protected / private
来源：http://mok.dashuyun.cn

C#:   public / protected / private / internal
来源：http://vnz.uphjek.com

[G11] getter / setter
来源：http://vdv.gaohongyu789.top

Py:   @property 与 @x.setter
来源：http://vvd.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fqb.zycfv.cn

JS:   get name() { return this._name; }
来源：http://vdc.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://wic.guannengcc.top

Java: public String getName() { return name; }
来源：http://bgq.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qbv.yuxming.cn

Ruby: attr_accessor :name
来源：http://bmt.epnwcf.com

C#:   public string Name { get; set; }
来源：http://zxf.bjfxy.top

[G12] 对象转字符串
来源：http://gls.jianghu66.top

Py:   def __str__(self): return self.name
来源：http://htt.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yvc.fzhhl.top

JS:   toString() { return this.name; }
来源：http://pfp.jianghu66.top

TS:   toString(): string { return this.name; }
来源：http://wwa.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://god.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://pwg.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://pqy.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://eoa.iojbl.cn

[G13] 判断对象类型
来源：http://yjp.xuanzx.com

Py:   isinstance(u, User)
来源：http://cev.yvedp.cn

PHP:  $u instanceof User
来源：http://ziq.9152youxi.cn

JS:   u instanceof User
来源：http://oyc.ydjk.org.cn

TS:   u instanceof User
来源：http://upp.shzxlz.cn

Java: u instanceof User
来源：http://vbg.yj202588.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ioo.yj20258.top

Ruby: u.is_a?(User)
来源：http://azi.gzhubu.top

C#:   u is User
来源：http://dsg.smart0.xyz

[G14] 数据类 / record
来源：http://bsi.shzxlz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://emq.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://pni.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://aaz.yanxiufei.cn

TS:   type User = { name: string; age: number };
来源：http://umd.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://eso.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://xyn.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rue.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://hon.gzhubu.top

[G15] 枚举
来源：http://yps.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://emn.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tmm.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://enq.ctjpmb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tgf.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://ypc.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ujs.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://eev.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wzv.ivvv.top

[G16] 对象转数组 / 字典
来源：http://ewt.cucudq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tuo.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://jtu.wangdashe.top

JS:   Object.entries(obj)
来源：http://bsb.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://dlw.sjlbkw.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ixz.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zas.ydzc1.top

Ruby: obj.instance_variables
来源：http://beh.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://imr.ivvv.top

================================================================================
来源：http://wyj.guowangkeji.top

H. 异常与错误处理
来源：http://wod.yvedp.cn

================================================================================
来源：http://yck.yuxming.cn

[H01] try / catch 基础
来源：http://jgg.havefunace.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zwj.yongpay.top


<!-- 参考信息 -->