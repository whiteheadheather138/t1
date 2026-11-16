代发 wailian999

Ruby: s.lines
来源：http://moy.zhongyouzk.top

C#:   s.Split('\n')
来源：http://ird.zhijiandao.cn

[E20] 判断字符串是否为空
来源：http://mdb.uphjek.com

Py:   if not s:
来源：http://hsq.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ftn.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://npx.pycfn.com

TS:   if (s === "") {}
来源：http://qtn.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://ysk.cucudq.cn

Go:   if s == "" {}
来源：http://plu.vehdjk.com

Ruby: if s.empty?
来源：http://wvy.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ikl.yj20258.top

[E21] 超长截断加省略号
来源：http://mzz.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yrs.wangdashe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pph.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xjn.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zkx.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rgf.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://tfc.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rws.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://riu.ydzc1.top

[E22] 字节长度与字符长度
来源：http://pmb.aizwys.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ikl.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ris.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uma.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://niy.epnwcf.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dkc.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rtw.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://pwe.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ocy.epnwcf.com

================================================================================
来源：http://hji.cdnleiting.top

F. 文件与目录
来源：http://prq.uphjek.com

================================================================================
来源：http://ihc.daria6918.cn

[F01] 读取整个文件
来源：http://wyt.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ztn.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://ecg.shangyingyoupin.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oll.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ohu.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kyn.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hpr.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://bgy.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://lvt.xuanzx.com

[F02] 逐行读取文件
来源：http://hms.havefunace.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uwy.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://edm.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nnr.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ibw.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://trq.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jxc.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kmr.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hyg.ehwqpu.com

[F03] 写入文件（覆盖）
来源：http://mei.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ufz.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zla.cucudq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://udq.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mnj.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iyq.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gxs.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://yex.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zmv.meibo888.top

[F04] 追加写入文件
来源：http://tto.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zti.zhixingplan.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://myi.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cqx.shangyingyoupin.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://smf.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dmb.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nfw.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ham.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rtb.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://yjs.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qpc.hongshengwenyu.top

PHP:  file_exists("a.txt");
来源：http://bcr.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://bae.snrcjt.cn

TS:   fs.existsSync("a.txt")
来源：http://mpn.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jys.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gwi.daxiang520.top

Ruby: File.exist?("a.txt")
来源：http://mbz.zhengqikj.top

C#:   File.Exists("a.txt")
来源：http://isd.gotoacloud.top

[F06] 删除文件
来源：http://oeh.xinyue.icu

Py:   os.remove("a.txt")
来源：http://qse.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://lyh.aizwys.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bfh.nwbrower.top

TS:   fs.unlinkSync("a.txt")
来源：http://yyb.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://brf.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://ago.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://are.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://iki.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://qsr.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lhp.fehbvm.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oln.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bsp.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hfz.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sra.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pby.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dsn.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hyc.sxryk.cn

[F08] 遍历目录
来源：http://szh.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://osh.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wwi.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://zth.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://uio.zdbjq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wem.jinqigfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tbh.meibo888.top

Ruby: Dir.children("dir")
来源：http://eit.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://mbs.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://cjo.c1oappe.top

Py:   os.path.getsize("a.txt")
来源：http://mgg.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://zgi.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://bor.redwolf501.top

TS:   fs.statSync("a.txt").size
来源：http://uuf.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://acn.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mjw.cheryme.top

Ruby: File.size("a.txt")
来源：http://pek.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://lql.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://bnz.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ahh.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nko.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lce.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://pxu.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vev.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wzk.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ltt.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ezg.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://eab.sxryk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fkl.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vpo.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://csf.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hkd.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://htx.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kqv.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pkk.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://npg.cashguo.top

[F12] CSV 读写
来源：http://eth.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uew.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tqn.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rqj.hywenlv.cn

TS:   // 同上
来源：http://yos.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qkx.sjlbkw.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bsa.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jvd.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ptl.gotoacloud.top

================================================================================
来源：http://qpv.zhijiandao.cn

G. 面向对象
来源：http://uav.sjlbkw.cn

================================================================================
来源：http://cdn.hcnkem.com

[G01] 定义类
来源：http://wel.jianghu66.top

Py:   class User: pass
来源：http://ems.hnxiangtu.top

PHP:  class User {}
来源：http://hox.xingfuxueyuan.xyz

JS:   class User {}
来源：http://myb.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://yli.gzhubu.top

Java: class User {}
来源：http://das.hammf.cn

Go:   type User struct { Name string }
来源：http://zqt.yuxming.cn

Ruby: class User; end
来源：http://ccv.nanxuanxn.top

C#:   class User {}
来源：http://mij.fengsongda.top

[G02] 构造函数
来源：http://xha.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://sii.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://kfp.shanyushiyangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://urd.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://xve.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://jrp.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rdc.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://lbz.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://ysi.sysykeji.top

[G03] 实例属性
来源：http://qow.daria6918.cn

Py:   self.name = "x"
来源：http://jto.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://ktr.quarkkingdee.top

JS:   this.name = "x";
来源：http://ifo.shangyingyoupin.top

TS:   name: string = "x";
来源：http://buv.shzxlz.cn

Java: private String name;
来源：http://wif.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tml.aizwys.cn

Ruby: @name = "x"
来源：http://xwp.guannengcc.top

C#:   public string Name { get; set; } = "x";
来源：http://xxq.gzhubu.top

[G04] 定义方法
来源：http://bdr.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://vkc.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://udy.xylfe.cn

JS:   greet() { return this.name; }
来源：http://tyr.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://lpv.sysykeji.top

Java: String greet() { return name; }
来源：http://htf.hcnkem.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://hnb.hnqzz.top

Ruby: def greet; @name; end
来源：http://alk.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://oqa.zhongyouzk.top

[G05] 继承
来源：http://ort.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://zsn.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://erc.chenzaomai.com

JS:   class Admin extends User {}
来源：http://cdo.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://rpi.yuxming.cn

Java: class Admin extends User {}
来源：http://egb.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qwy.ydjk.org.cn

Ruby: class Admin < User; end
来源：http://zfv.jiagoushi.top

C#:   class Admin : User {}
来源：http://cca.haohaochexian.top

[G06] 重写方法
来源：http://flo.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://efn.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://wnz.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://ide.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://cpu.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://qrx.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iin.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://jui.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://oxo.chenzaomai.com

[G07] 调用父类方法
来源：http://yyp.zdbjq.cn

Py:   super().greet()
来源：http://qjc.yj202588.top

PHP:  parent::greet();
来源：http://qgf.tianlin.xyz

JS:   super.greet();
来源：http://gqw.jiagoushi.top

TS:   super.greet();
来源：http://woq.vehdjk.com

Java: super.greet();
来源：http://hus.yueranfly.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fby.kuanghao11.cn

Ruby: super
来源：http://ild.xziqi.cn

C#:   base.Greet();
来源：http://fay.xziqi.cn

[G08] 静态方法与属性
来源：http://wwa.chenjidiqi.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kwf.pycfn.com

PHP:  public static function f() {}
来源：http://szd.quarkkingdee.top

JS:   static f() {}
来源：http://uvx.gzhubu.top

TS:   static f(): void {}
来源：http://dzk.hywenlv.cn

Java: static void f() {}
来源：http://xcu.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://zyg.gogol.net.cn

Ruby: def self.f; end
来源：http://xkz.yvedp.cn

C#:   public static void F() {}
来源：http://yuo.tianlin.xyz

[G09] 接口 / 抽象类
来源：http://ijd.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://ceu.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://yln.shzxlz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yhi.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://coz.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://bki.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://vmr.jqgfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kze.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://jcv.gzhubu.top

[G10] 访问控制
来源：http://bll.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://emu.9152youxi.cn

PHP:  public / protected / private
来源：http://msb.zycfv.cn

JS:   #private 字段；其余公开
来源：http://zmd.mhx1999.top

TS:   public / protected / private
来源：http://wkk.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://jrd.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vmt.yj202588.top

Ruby: public / protected / private
来源：http://gqr.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://cdc.fanxiaobao.xyz

[G11] getter / setter
来源：http://nek.chenlongwang.top

Py:   @property 与 @x.setter
来源：http://nvy.nwbrower.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vkx.meibo888.top

JS:   get name() { return this._name; }
来源：http://wse.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://ook.cheryme.top

Java: public String getName() { return name; }
来源：http://mxm.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yhd.andypj.xyz

Ruby: attr_accessor :name
来源：http://uee.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://hpi.xylfe.cn

[G12] 对象转字符串
来源：http://xyf.havefunace.top

Py:   def __str__(self): return self.name
来源：http://tjs.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xje.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://zpv.jinqigufen.top

TS:   toString(): string { return this.name; }
来源：http://wcu.ctjpmb.com

Java: @Override public String toString() { return name; }
来源：http://pji.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hyn.cucudq.cn

Ruby: def to_s; @name; end
来源：http://trh.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://pel.sjlbkw.cn

[G13] 判断对象类型
来源：http://gcr.hesvh.cn

Py:   isinstance(u, User)
来源：http://mfi.316326.xyz

PHP:  $u instanceof User
来源：http://ptw.xuanzx.com

JS:   u instanceof User
来源：http://nli.ywan-chungtsiang.top

TS:   u instanceof User
来源：http://fmc.ivvv.top

Java: u instanceof User
来源：http://tbi.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yat.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://lbr.xingfuxueyuan.xyz

C#:   u is User
来源：http://nnr.cheryme.top

[G14] 数据类 / record
来源：http://fhc.fanxiaobao.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qth.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://xrs.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://ngt.iojbl.cn

TS:   type User = { name: string; age: number };
来源：http://qfq.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://uqi.xuetiantiany.cn

Go:   type User struct { Name string; Age int }
来源：http://bqn.redwolf501.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xga.yueranfly.top

C#:   record User(string Name, int Age);
来源：http://bvo.vqdsnc.cn

[G15] 枚举
来源：http://olr.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://epa.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ond.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vvh.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rhi.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://lky.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fpc.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://efu.shanyushiyangtech.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://anb.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://mqt.sxryk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vwd.cdnleiting.top

PHP:  get_object_vars($obj);
来源：http://vne.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://pgm.cdnleiting.top

TS:   Object.entries(obj)
来源：http://emu.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uar.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://urb.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://dfc.ehwqpu.com

C#:   // 用反射或 System.Text.Json
来源：http://cpw.zhiwuduotai.top

================================================================================
来源：http://aby.jianghu66.top

H. 异常与错误处理
来源：http://jyc.quarkkingdee.top

================================================================================
来源：http://xkq.yfazqb.com

[H01] try / catch 基础
来源：http://efp.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pgb.yj20258.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rqs.cqqwz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lbk.birdmap.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vta.fehbvm.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://atj.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gzr.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mib.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bel.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://put.yj20258.top


<!-- 参考信息 -->