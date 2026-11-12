代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lvo.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wik.hcnkem.com

TS:   if (s === "") {}
来源：http://bsf.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://yam.daxiang520.top

Go:   if s == "" {}
来源：http://gpl.gotoacloud.top

Ruby: if s.empty?
来源：http://uvf.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qks.ppjwa.cn

[E21] 超长截断加省略号
来源：http://pcb.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ddp.zhoulong.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aly.nanxinkj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gbh.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mit.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zsg.cucudq.cn

Go:   // 按 rune 判断长度后截断
来源：http://ydx.ydjk.org.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qbw.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dym.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://gso.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://boo.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bxh.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mhw.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yix.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oew.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yvu.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://jzw.zhiwuduotai.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nie.yuxming.cn

================================================================================
来源：http://aek.jianghu66.top

F. 文件与目录
来源：http://knj.guowangkeji.top

================================================================================
来源：http://ykm.zdbjq.cn

[F01] 读取整个文件
来源：http://bdm.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tay.gaohongyu789.top

PHP:  file_get_contents("a.txt");
来源：http://aow.xziqi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dec.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rym.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://wmq.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wqm.kuanghao11.cn

Ruby: File.read("a.txt")
来源：http://htp.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://xqx.nanxinkj.top

[F02] 逐行读取文件
来源：http://uqd.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://elq.ehwqpu.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aac.zhijiandao.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rpx.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://teh.hammf.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://evi.jinghuilouyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tcb.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nqf.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pyn.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://hol.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hpw.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lvz.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vva.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ovb.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vdq.shzxlz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rcf.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://wrm.hnxiangtu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iyr.shuidangran.top

[F04] 追加写入文件
来源：http://xib.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yfc.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://aus.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oqg.mhx1999.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jqn.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vjr.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vmz.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://chn.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hqx.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://flh.guowangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fpv.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://tqt.sxryk.cn

JS:   fs.existsSync("a.txt")
来源：http://uby.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://mrt.tian-w.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vlm.gzhubu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://val.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://zbi.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://xka.daria6918.cn

[F06] 删除文件
来源：http://ycm.nwbrower.top

Py:   os.remove("a.txt")
来源：http://yxv.bbcook.cn

PHP:  unlink("a.txt");
来源：http://msu.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://iqg.fktsv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qjs.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jwp.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://hgt.nwbrower.top

Ruby: File.delete("a.txt")
来源：http://qha.316326.xyz

C#:   File.Delete("a.txt");
来源：http://pfb.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://ylj.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lcq.chenzaomai.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nns.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ygu.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ocg.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://utn.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ylo.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eln.shuidangran.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rov.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://qvl.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://veb.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jgl.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://fxj.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://vto.zdbjq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vws.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kgn.hcnkem.com

Ruby: Dir.children("dir")
来源：http://zcf.redwolf501.top

C#:   Directory.GetFiles("dir")
来源：http://svt.zhengqikj.top

[F09] 获取文件大小
来源：http://fmx.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://ofi.zhiwuduotai.top

PHP:  filesize("a.txt");
来源：http://zno.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://xhm.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://qze.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ioh.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tam.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://tyh.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://ocb.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://jvf.vqdsnc.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sci.fktsv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uqm.bbcook.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dhd.meibo888.top

TS:   path.extname("a.txt")
来源：http://noz.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vjy.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aao.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gze.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nlq.fzhhl.top

[F11] 复制与移动文件
来源：http://ywu.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rvw.jlsjyb.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lul.yj20258.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bia.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hkz.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cid.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://szw.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qaf.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jvo.yangfankeji.com

[F12] CSV 读写
来源：http://ojy.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mng.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uth.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://upa.gogol.net.cn

TS:   // 同上
来源：http://qjo.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ivt.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gjs.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ucv.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://byj.zhengqikj.top

================================================================================
来源：http://uko.shuidangran.top

G. 面向对象
来源：http://ffq.chenlongwang.top

================================================================================
来源：http://okw.chenzaomai.com

[G01] 定义类
来源：http://rzm.jinqigfzy.top

Py:   class User: pass
来源：http://fjz.zhoulong.xyz

PHP:  class User {}
来源：http://zlu.aibaodan.cn

JS:   class User {}
来源：http://bdp.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://agk.chenzaomai.com

Java: class User {}
来源：http://qel.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://hmy.jlsjyb.cn

Ruby: class User; end
来源：http://kxf.zhixingplan.top

C#:   class User {}
来源：http://sws.yuanzhike.top

[G02] 构造函数
来源：http://wzu.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://hmu.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://tfx.ywan-chungtsiang.top

JS:   constructor(name) { this.name = name; }
来源：http://fmf.aizwys.cn

TS:   constructor(public name: string) {}
来源：http://zbc.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://wxj.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rxn.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://chs.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://eml.jqgufenzy.top

[G03] 实例属性
来源：http://cdr.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://slq.jianghu66.top

PHP:  public string $name = "x";
来源：http://mnq.yj20258888.top

JS:   this.name = "x";
来源：http://eew.52xcode.cn

TS:   name: string = "x";
来源：http://crk.cucudq.cn

Java: private String name;
来源：http://loc.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pol.jinqigfzy.top

Ruby: @name = "x"
来源：http://jyb.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://wrs.hammf.cn

[G04] 定义方法
来源：http://rpp.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://nhr.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://atd.cheryme.top

JS:   greet() { return this.name; }
来源：http://acy.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://rlw.0kj1m.cn

Java: String greet() { return name; }
来源：http://tih.yuanzhike.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pre.c1oappe.top

Ruby: def greet; @name; end
来源：http://nzw.fengsongda.top

C#:   public string Greet() => Name;
来源：http://xiv.aibaodan.cn

[G05] 继承
来源：http://wth.yfazqb.com

Py:   class Admin(User): pass
来源：http://gwm.sxryk.cn

PHP:  class Admin extends User {}
来源：http://gby.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://hvk.hammf.cn

TS:   class Admin extends User {}
来源：http://rqf.mhx1999.top

Java: class Admin extends User {}
来源：http://ujp.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mlt.jqgufenzy.top

Ruby: class Admin < User; end
来源：http://nhf.uphjek.com

C#:   class Admin : User {}
来源：http://vxo.nanxuanxn.top

[G06] 重写方法
来源：http://iht.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://kpa.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zmy.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://bsc.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://pwl.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://mtf.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ikc.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://mob.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://ejc.ctjpmb.com

[G07] 调用父类方法
来源：http://asp.sxryk.cn

Py:   super().greet()
来源：http://psn.epnwcf.com

PHP:  parent::greet();
来源：http://wjn.quarkkingdee.top

JS:   super.greet();
来源：http://bmv.yj20258.top

TS:   super.greet();
来源：http://lqk.cheryme.top

Java: super.greet();
来源：http://zmq.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lvr.xuanzx.com

Ruby: super
来源：http://zed.zycfv.cn

C#:   base.Greet();
来源：http://tan.yangfankeji.com

[G08] 静态方法与属性
来源：http://jri.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ysh.uphjek.com

PHP:  public static function f() {}
来源：http://hzc.zhaomingkeji.xyz

JS:   static f() {}
来源：http://jof.jinqigfzy.top

TS:   static f(): void {}
来源：http://wvb.hysaishi.cn

Java: static void f() {}
来源：http://izm.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nhy.hfpthk.cn

Ruby: def self.f; end
来源：http://rre.wangdashe.top

C#:   public static void F() {}
来源：http://asb.vehdjk.com

[G09] 接口 / 抽象类
来源：http://ivm.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://kcr.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://jji.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pmr.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://yui.fengsongda.top

Java: interface Shape { double area(); }
来源：http://jbp.yangfankeji.com

Go:   type Shape interface { Area() float64 }
来源：http://uct.ybcxt.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qub.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://hnx.fengsongda.top

[G10] 访问控制
来源：http://gcx.yuxming.cn

Py:   约定 _protected / __private（不强制）
来源：http://oze.wangdashe.top

PHP:  public / protected / private
来源：http://zsw.epnwcf.com

JS:   #private 字段；其余公开
来源：http://ewn.yuxming.cn

TS:   public / protected / private
来源：http://dfu.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://cwx.daxiang520.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wws.aizwys.cn

Ruby: public / protected / private
来源：http://muk.tarul.cn

C#:   public / protected / private / internal
来源：http://vuw.0kj1m.cn

[G11] getter / setter
来源：http://gcj.tarul.cn

Py:   @property 与 @x.setter
来源：http://tka.fktsv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bcs.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://uca.ppjwa.cn

TS:   get name(): string { return this._name; }
来源：http://lrb.ywan-chungtsiang.top

Java: public String getName() { return name; }
来源：http://geu.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dji.ivvv.top

Ruby: attr_accessor :name
来源：http://lkf.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://ycr.0kj1m.cn

[G12] 对象转字符串
来源：http://lek.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://gjd.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://dtt.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://nkb.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://jpc.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://txm.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bff.hesvh.cn

Ruby: def to_s; @name; end
来源：http://eps.havefunace.top

C#:   public override string ToString() => Name;
来源：http://xrt.tarul.cn

[G13] 判断对象类型
来源：http://clo.chenjidiqi.icu

Py:   isinstance(u, User)
来源：http://wrt.jianghu66.top

PHP:  $u instanceof User
来源：http://gxk.sweek.top

JS:   u instanceof User
来源：http://tnv.52xcode.cn

TS:   u instanceof User
来源：http://noy.chenjidiqi.icu

Java: u instanceof User
来源：http://bht.smart0.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://asc.fehbvm.com

Ruby: u.is_a?(User)
来源：http://clf.hongshengwenyu.top

C#:   u is User
来源：http://pek.cheryme.top

[G14] 数据类 / record
来源：http://ynn.yj202588.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oxz.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://dxp.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://xar.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://psh.xylfe.cn

Java: record User(String name, int age) {}
来源：http://wvf.tarul.cn

Go:   type User struct { Name string; Age int }
来源：http://hdc.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dno.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://abb.yuanzhike.top

[G15] 枚举
来源：http://jqp.fengsongda.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jfz.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://asl.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uzx.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://exq.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://hzn.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ihk.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://cxq.xingfuxueyuan.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ene.cashguo.top

[G16] 对象转数组 / 字典
来源：http://rwm.dashuyun.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jkg.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://cti.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://pva.daxiang520.top

TS:   Object.entries(obj)
来源：http://vwz.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cpj.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ner.zhoulong.xyz

Ruby: obj.instance_variables
来源：http://kiy.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://vwj.guowangkeji.top

================================================================================
来源：http://pzg.sweek.top

H. 异常与错误处理
来源：http://fol.ctjpmb.com

================================================================================
来源：http://oru.shuidangran.top

[H01] try / catch 基础
来源：http://aon.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jil.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://enr.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bed.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xzt.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wsf.ctjpmb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://spw.ctjpmb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cgh.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ego.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://oft.uphjek.com

Py:   try: f()⏎finally: cleanup()
来源：http://djx.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ban.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://bil.svipenyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zcu.andypj.xyz


<!-- 参考信息 -->