代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jrz.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://wdq.dashuyun.cn

Py:   s.splitlines()
来源：http://vzx.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wca.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://xkz.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://rtd.meibo888.top

Java: s.lines().toList()
来源：http://mka.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://kfa.zycfv.cn

Ruby: s.lines
来源：http://yjx.ydzc1.top

C#:   s.Split('\n')
来源：http://otu.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://ayx.jqgufenzy.top

Py:   if not s:
来源：http://pcx.mhx1999.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wdq.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jsw.redwolf501.top

TS:   if (s === "") {}
来源：http://mcf.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://ivh.xinyue.icu

Go:   if s == "" {}
来源：http://mxb.andypj.xyz

Ruby: if s.empty?
来源：http://gca.hammf.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ksi.hywenlv.cn

[E21] 超长截断加省略号
来源：http://bzz.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xbr.meibo888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hxq.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dac.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vrk.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kqp.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://tit.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xar.chenzaomai.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yjg.sysykeji.top

[E22] 字节长度与字符长度
来源：http://jez.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ecw.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ein.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pve.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xrj.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hyx.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tot.yj202588.top

Ruby: s.bytesize;  s.length
来源：http://pwd.hysaishi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vye.svipenyu.cn

================================================================================
来源：http://xxh.yuxming.cn

F. 文件与目录
来源：http://def.ivvv.top

================================================================================
来源：http://hcx.gogol.net.cn

[F01] 读取整个文件
来源：http://zsh.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nqe.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://mdb.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fjp.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ftg.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://prn.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yqg.havefunace.top

Ruby: File.read("a.txt")
来源：http://spj.shanyushiyangtech.top

C#:   File.ReadAllText("a.txt");
来源：http://cdw.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://nwl.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://llf.ybcxt.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://quk.hesvh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://swc.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wrq.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gbl.meibo888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cvv.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ovg.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rpk.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://nsr.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uof.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gmo.9152youxi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oyo.xinyue.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wxz.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qtr.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kar.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://ibz.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://san.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://pgu.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mke.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hzi.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bxa.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://idm.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ozs.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jwi.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yuv.fehbvm.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vpe.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://juj.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kkc.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://jsx.c1oappe.top

JS:   fs.existsSync("a.txt")
来源：http://qfh.xziqi.cn

TS:   fs.existsSync("a.txt")
来源：http://hvg.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mym.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vdv.smart0.xyz

Ruby: File.exist?("a.txt")
来源：http://ntu.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://uvz.iojbl.cn

[F06] 删除文件
来源：http://zxd.yj20258.top

Py:   os.remove("a.txt")
来源：http://lfg.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://acw.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://dap.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hpr.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pih.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://jeb.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://sxh.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://rht.aizwys.cn

[F07] 创建目录（含多级）
来源：http://utk.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qxs.gzhubu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nrs.yj202588.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://onw.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dql.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kly.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bwk.dashuyun.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://btc.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nfr.nwbrower.top

[F08] 遍历目录
来源：http://opl.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://xor.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tpq.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://jmm.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://vfj.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sio.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://upp.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://maf.aibaodan.cn

C#:   Directory.GetFiles("dir")
来源：http://jcq.pycfn.com

[F09] 获取文件大小
来源：http://phg.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://hse.nanxinkj.top

PHP:  filesize("a.txt");
来源：http://fcc.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://dyr.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://zww.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://szn.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bcn.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://rxl.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://vkw.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://huk.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ptd.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ezu.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kxy.shuidangran.top

TS:   path.extname("a.txt")
来源：http://wre.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ubt.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dpd.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zjq.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ufi.zhixingplan.top

[F11] 复制与移动文件
来源：http://vrq.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vec.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rks.cdnleiting.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tcv.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://imd.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ffe.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tci.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ppy.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vaz.xuanzx.com

[F12] CSV 读写
来源：http://vse.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vvj.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oqz.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kqa.52xcode.cn

TS:   // 同上
来源：http://gqx.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ulm.shzxlz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://laa.snrcjt.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cuo.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rrl.cashguo.top

================================================================================
来源：http://eww.9152youxi.cn

G. 面向对象
来源：http://jml.ydjk.org.cn

================================================================================
来源：http://epg.pycfn.com

[G01] 定义类
来源：http://xmq.yvedp.cn

Py:   class User: pass
来源：http://cnq.yuanzhike.top

PHP:  class User {}
来源：http://erp.tanke756.top

JS:   class User {}
来源：http://pvi.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://sju.gotoacloud.top

Java: class User {}
来源：http://knk.hnqzz.top

Go:   type User struct { Name string }
来源：http://jhc.9152youxi.cn

Ruby: class User; end
来源：http://qdx.daria6918.cn

C#:   class User {}
来源：http://fgn.gaohongyu789.top

[G02] 构造函数
来源：http://waq.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://hte.shanyushiyangtech.top

PHP:  public function __construct(public string $name) {}
来源：http://bne.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://ufr.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://iia.jlsjyb.cn

Java: User(String name) { this.name = name; }
来源：http://mkb.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fsq.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://vnx.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://exo.cucudq.cn

[G03] 实例属性
来源：http://fqp.hfpthk.cn

Py:   self.name = "x"
来源：http://loa.yongpay.top

PHP:  public string $name = "x";
来源：http://ypd.mhx1999.top

JS:   this.name = "x";
来源：http://pjr.jqgfzy.top

TS:   name: string = "x";
来源：http://ydk.hammf.cn

Java: private String name;
来源：http://lgi.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ois.ehwqpu.com

Ruby: @name = "x"
来源：http://itp.shanyushiyangtech.top

C#:   public string Name { get; set; } = "x";
来源：http://woo.yonumen.top

[G04] 定义方法
来源：http://jpg.zycfv.cn

Py:   def greet(self): return self.name
来源：http://pif.quarkkingdee.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qcw.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://jwe.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://mxb.wangdashe.top

Java: String greet() { return name; }
来源：http://yxo.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ksy.jinqigufen.top

Ruby: def greet; @name; end
来源：http://rmw.hammf.cn

C#:   public string Greet() => Name;
来源：http://ivk.vehdjk.com

[G05] 继承
来源：http://xkt.ydjk.org.cn

Py:   class Admin(User): pass
来源：http://lrx.nwbrower.top

PHP:  class Admin extends User {}
来源：http://gsi.birdmap.top

JS:   class Admin extends User {}
来源：http://wxi.0kj1m.cn

TS:   class Admin extends User {}
来源：http://tjl.shzxlz.cn

Java: class Admin extends User {}
来源：http://lna.shangyingyoupin.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wno.sufxvd.cn

Ruby: class Admin < User; end
来源：http://rth.jlsjyb.cn

C#:   class Admin : User {}
来源：http://zvi.dashuyun.cn

[G06] 重写方法
来源：http://vvi.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://kdk.yj20258888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tmq.ehwqpu.com

JS:   greet() { return "admin"; }
来源：http://hyi.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://scs.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://nuw.cucudq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ssn.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://tms.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://bgt.fengsongda.top

[G07] 调用父类方法
来源：http://wdl.wangshuangyany.cn

Py:   super().greet()
来源：http://wks.shangyingyoupin.top

PHP:  parent::greet();
来源：http://agn.snrcjt.cn

JS:   super.greet();
来源：http://lot.fengsongda.top

TS:   super.greet();
来源：http://ilg.jqgufenzy.top

Java: super.greet();
来源：http://kqh.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://had.zhengqikj.top

Ruby: super
来源：http://nvw.sysykeji.top

C#:   base.Greet();
来源：http://tyd.jqgfzy.top

[G08] 静态方法与属性
来源：http://dxs.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yct.yanxiufei.cn

PHP:  public static function f() {}
来源：http://bxy.kuanghao11.cn

JS:   static f() {}
来源：http://aeg.jyoumei.cn

TS:   static f(): void {}
来源：http://ujd.xingfuxueyuan.xyz

Java: static void f() {}
来源：http://lej.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ypc.nanxuanxn.top

Ruby: def self.f; end
来源：http://beg.tian-w.cn

C#:   public static void F() {}
来源：http://hfm.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://pry.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://lxb.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pjg.zhoulong.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://cig.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://wba.epnwcf.com

Java: interface Shape { double area(); }
来源：http://ajd.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://nxe.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qkw.hnxiangtu.top

C#:   interface IShape { double Area(); }
来源：http://xti.tanke756.top

[G10] 访问控制
来源：http://czh.yj20258.top

Py:   约定 _protected / __private（不强制）
来源：http://qph.jinyuanbaomall.cn

PHP:  public / protected / private
来源：http://rml.52xcode.cn

JS:   #private 字段；其余公开
来源：http://nxh.yj20258888.top

TS:   public / protected / private
来源：http://xyv.yvedp.cn

Java: public / protected / private / 默认包级
来源：http://isf.cqqwz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://erw.yfazqb.com

Ruby: public / protected / private
来源：http://nqe.gotoacloud.top

C#:   public / protected / private / internal
来源：http://pfl.316326.xyz

[G11] getter / setter
来源：http://hha.shuidangran.top

Py:   @property 与 @x.setter
来源：http://ugi.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://fwe.iojbl.cn

JS:   get name() { return this._name; }
来源：http://bot.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://ydf.ybcxt.top

Java: public String getName() { return name; }
来源：http://ady.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sxh.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://ago.bjfxy.top

C#:   public string Name { get; set; }
来源：http://oql.ivvv.top

[G12] 对象转字符串
来源：http://vzj.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://qww.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eqv.fehbvm.com

JS:   toString() { return this.name; }
来源：http://gra.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://eto.hammf.cn

Java: @Override public String toString() { return name; }
来源：http://fmn.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://wdj.shuidangran.top

Ruby: def to_s; @name; end
来源：http://acr.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://mhx.yueranfly.top

[G13] 判断对象类型
来源：http://auw.fehbvm.com

Py:   isinstance(u, User)
来源：http://bmd.jiagoushi.top

PHP:  $u instanceof User
来源：http://aql.jqgfzy.top

JS:   u instanceof User
来源：http://gcs.yongpay.top

TS:   u instanceof User
来源：http://tiu.ydzc1.top

Java: u instanceof User
来源：http://tkr.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://pse.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://gzs.xingfuxueyuan.xyz

C#:   u is User
来源：http://fnz.tanke756.top

[G14] 数据类 / record
来源：http://eyz.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xsv.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://rap.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://dms.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://jju.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://yww.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://pgz.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xom.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://xsy.c1oappe.top

[G15] 枚举
来源：http://qqy.zhongyouzk.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ktr.hfpthk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jux.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gyz.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qxl.c1oappe.top

Java: enum Color { RED, GREEN }
来源：http://oeu.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rlq.sweek.top

Ruby: Color = %i[red green].freeze
来源：http://wqs.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wwr.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://taf.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bwo.zhiwuduotai.top

PHP:  get_object_vars($obj);
来源：http://mid.dianchejie.cn

JS:   Object.entries(obj)
来源：http://bur.fktsv.cn

TS:   Object.entries(obj)
来源：http://fnj.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kij.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tbu.yongpay.top

Ruby: obj.instance_variables
来源：http://ugl.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://iya.bbcook.cn

================================================================================
来源：http://uhz.shzxlz.cn

H. 异常与错误处理
来源：http://jme.shangyingyoupin.top

================================================================================
来源：http://uri.shzxlz.cn

[H01] try / catch 基础
来源：http://gnw.fzhhl.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://plm.hcnkem.com


<!-- 参考信息 -->