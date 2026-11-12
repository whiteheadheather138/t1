代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://egf.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://swu.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://iyy.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://lcs.wangshuangyany.cn

Go:   if s == "" {}
来源：http://vxr.hesvh.cn

Ruby: if s.empty?
来源：http://jyl.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://slr.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://atx.jinqigufen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uhu.meibo888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hop.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tlu.shzxlz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fnz.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://foa.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://lzl.andypj.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tqn.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://isl.hammf.cn

[E22] 字节长度与字符长度
来源：http://vuz.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vir.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kan.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bgx.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://egg.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bga.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yej.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://oqi.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qki.daxiang520.top

================================================================================
来源：http://qyw.zdqjudy.top

F. 文件与目录
来源：http://tmj.ppjwa.cn

================================================================================
来源：http://cnb.aibaodan.cn

[F01] 读取整个文件
来源：http://efk.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uea.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://tdc.yanxiufei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mzp.andypj.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://acc.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://usr.yj20258888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jjv.andypj.xyz

Ruby: File.read("a.txt")
来源：http://mjp.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://xnr.hcnkem.com

[F02] 逐行读取文件
来源：http://vgd.snrcjt.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://amk.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ifw.ydzc1.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lkm.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://opf.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ash.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hut.shzxlz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cwd.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zhw.cheryme.top

[F03] 写入文件（覆盖）
来源：http://chy.gzhubu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zks.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://tue.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ata.wangshuangyany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pqw.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ufg.pengpengdd.cyou

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uiw.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://wkb.shanyushiyangtech.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iym.hammf.cn

[F04] 追加写入文件
来源：http://yjf.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rcd.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://okw.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sba.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fgd.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ugb.sweek.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nll.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rud.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mlp.9152youxi.cn

[F05] 判断文件或目录是否存在
来源：http://syb.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://czq.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://vtv.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://tqp.yfazqb.com

TS:   fs.existsSync("a.txt")
来源：http://fbp.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ivu.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sfs.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://qnz.pycfn.com

C#:   File.Exists("a.txt")
来源：http://brr.xuanzx.com

[F06] 删除文件
来源：http://fxv.yuxming.cn

Py:   os.remove("a.txt")
来源：http://vdv.daria6918.cn

PHP:  unlink("a.txt");
来源：http://erz.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://hyg.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://zbu.hongshengwenyu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://viz.pengpengdd.cyou

Go:   os.Remove("a.txt")
来源：http://nkh.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://ylo.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://vio.hfpthk.cn

[F07] 创建目录（含多级）
来源：http://epu.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tgq.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wnm.yj20258888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://axz.ehwqpu.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gcu.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ojv.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gso.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ysr.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tau.fanxiaobao.xyz

[F08] 遍历目录
来源：http://cgk.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://xce.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cjb.jiagoushi.top

JS:   fs.readdirSync("dir")
来源：http://gku.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://nok.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hko.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tpc.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://ith.nanxinkj.top

C#:   Directory.GetFiles("dir")
来源：http://mgu.xylfe.cn

[F09] 获取文件大小
来源：http://itt.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://bys.hesvh.cn

PHP:  filesize("a.txt");
来源：http://gim.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://aot.jinqigfzy.top

TS:   fs.statSync("a.txt").size
来源：http://yuf.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://ayi.chenlongwang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ccu.shuidangran.top

Ruby: File.size("a.txt")
来源：http://uml.fehbvm.com

C#:   new FileInfo("a.txt").Length
来源：http://dtw.jqgfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://qok.vqdsnc.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ude.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://snf.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wkn.smart0.xyz

TS:   path.extname("a.txt")
来源：http://baw.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eoh.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fuq.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gmz.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kxh.bjfxy.top

[F11] 复制与移动文件
来源：http://tye.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nmw.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://btf.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ntg.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cqv.dashuyun.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yqx.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://anz.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lbp.zdqjudy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ttg.feifeiyinyue.top

[F12] CSV 读写
来源：http://bbc.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wuy.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vpj.tian-w.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xcv.daria6918.cn

TS:   // 同上
来源：http://idx.ctjpmb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kbb.jinqigfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oie.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mqu.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jzz.gotoacloud.top

================================================================================
来源：http://lvh.xuetiantiany.cn

G. 面向对象
来源：http://abe.haohaochexian.top

================================================================================
来源：http://tug.c1oappe.top

[G01] 定义类
来源：http://mag.ywan-chungtsiang.top

Py:   class User: pass
来源：http://xhd.52xcode.cn

PHP:  class User {}
来源：http://grb.xuetiantiany.cn

JS:   class User {}
来源：http://lea.smart0.xyz

TS:   class User { name: string = ""; }
来源：http://een.hnxiangtu.top

Java: class User {}
来源：http://khn.fktsv.cn

Go:   type User struct { Name string }
来源：http://zmg.hysaishi.cn

Ruby: class User; end
来源：http://sdj.ctjpmb.com

C#:   class User {}
来源：http://hsx.bbcook.cn

[G02] 构造函数
来源：http://iut.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://lwc.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://pbi.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://grq.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://qkh.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://kwz.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lux.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://tma.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://ctz.cucudq.cn

[G03] 实例属性
来源：http://hwr.sufxvd.cn

Py:   self.name = "x"
来源：http://tbe.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://wxd.sxryk.cn

JS:   this.name = "x";
来源：http://wcr.yvedp.cn

TS:   name: string = "x";
来源：http://gwb.gogol.net.cn

Java: private String name;
来源：http://qpx.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lck.jiagoushi.top

Ruby: @name = "x"
来源：http://jeh.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://vkx.jianghu66.top

[G04] 定义方法
来源：http://pwr.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://klk.vqdsnc.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bqt.ydjk.org.cn

JS:   greet() { return this.name; }
来源：http://seb.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://qty.ppjwa.cn

Java: String greet() { return name; }
来源：http://fjt.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hlq.chenlongwang.top

Ruby: def greet; @name; end
来源：http://nvh.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://xmo.fktsv.cn

[G05] 继承
来源：http://rnr.nwbrower.top

Py:   class Admin(User): pass
来源：http://tts.cashguo.top

PHP:  class Admin extends User {}
来源：http://knt.jiagoushi.top

JS:   class Admin extends User {}
来源：http://vog.jqgfzy.top

TS:   class Admin extends User {}
来源：http://utd.svipenyu.cn

Java: class Admin extends User {}
来源：http://fan.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kny.xuanzx.com

Ruby: class Admin < User; end
来源：http://zzp.xingfuxueyuan.xyz

C#:   class Admin : User {}
来源：http://ukl.ydjk.org.cn

[G06] 重写方法
来源：http://ckr.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://uum.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ucb.birdmap.top

JS:   greet() { return "admin"; }
来源：http://mcx.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://xvp.316326.xyz

Java: @Override String greet() { return "admin"; }
来源：http://bes.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yew.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://xfy.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://mvs.zhongyouzk.top

[G07] 调用父类方法
来源：http://oup.nwbrower.top

Py:   super().greet()
来源：http://fiu.fengsongda.top

PHP:  parent::greet();
来源：http://vmo.gaohongyu789.top

JS:   super.greet();
来源：http://akd.fengsongda.top

TS:   super.greet();
来源：http://xjj.yfazqb.com

Java: super.greet();
来源：http://cxs.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ssr.hnxiangtu.top

Ruby: super
来源：http://nyp.gzhubu.top

C#:   base.Greet();
来源：http://yaj.hcnkem.com

[G08] 静态方法与属性
来源：http://iin.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iuz.jinqigfzy.top

PHP:  public static function f() {}
来源：http://sxj.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://znv.zdbjq.cn

TS:   static f(): void {}
来源：http://zvi.0kj1m.cn

Java: static void f() {}
来源：http://ptn.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gyp.havefunace.top

Ruby: def self.f; end
来源：http://jqg.guannengcc.top

C#:   public static void F() {}
来源：http://sey.xziqi.cn

[G09] 接口 / 抽象类
来源：http://uil.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://muc.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://alq.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nyu.xuetiantiany.cn

TS:   interface Shape { area(): number; }
来源：http://trc.gotoacloud.top

Java: interface Shape { double area(); }
来源：http://uzw.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://ror.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ulx.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://qmk.gzhubu.top

[G10] 访问控制
来源：http://xxg.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://wwm.redwolf501.top

PHP:  public / protected / private
来源：http://epz.ydzc1.top

JS:   #private 字段；其余公开
来源：http://ere.svipenyu.cn

TS:   public / protected / private
来源：http://zpp.cqqwz.cn

Java: public / protected / private / 默认包级
来源：http://fke.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://icl.jinqigfzy.top

Ruby: public / protected / private
来源：http://upz.mhx1999.top

C#:   public / protected / private / internal
来源：http://pfo.52xcode.cn

[G11] getter / setter
来源：http://ryw.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://sma.shangyingyoupin.top

PHP:  public function getName(): string { return $this->name; }
来源：http://adf.yongpay.top

JS:   get name() { return this._name; }
来源：http://vcd.yanxiufei.cn

TS:   get name(): string { return this._name; }
来源：http://tdl.nwbrower.top

Java: public String getName() { return name; }
来源：http://yzi.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yyl.daria6918.cn

Ruby: attr_accessor :name
来源：http://kxi.ehwqpu.com

C#:   public string Name { get; set; }
来源：http://zsj.vqdsnc.cn

[G12] 对象转字符串
来源：http://gbl.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://dbl.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ofc.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://hij.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://eba.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://lwd.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rgb.zhongyouzk.top

Ruby: def to_s; @name; end
来源：http://anc.yj202588.top

C#:   public override string ToString() => Name;
来源：http://rft.cashguo.top

[G13] 判断对象类型
来源：http://lrs.yj20258888.top

Py:   isinstance(u, User)
来源：http://xpi.chenjidiqi.icu

PHP:  $u instanceof User
来源：http://hyl.sysykeji.top

JS:   u instanceof User
来源：http://yju.yueranfly.top

TS:   u instanceof User
来源：http://iee.ydzc1.top

Java: u instanceof User
来源：http://hmd.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uwa.sweek.top

Ruby: u.is_a?(User)
来源：http://zvk.xylfe.cn

C#:   u is User
来源：http://tkq.xylfe.cn

[G14] 数据类 / record
来源：http://ftn.gaohongyu789.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://spb.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://hnb.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lje.zhaomingkeji.xyz

TS:   type User = { name: string; age: number };
来源：http://reg.tianlin.xyz

Java: record User(String name, int age) {}
来源：http://jrd.yj202588.top

Go:   type User struct { Name string; Age int }
来源：http://xye.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qrf.havefunace.top

C#:   record User(string Name, int Age);
来源：http://owq.cdnleiting.top

[G15] 枚举
来源：http://swr.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://swe.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://acb.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://srv.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rmu.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://url.epnwcf.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kjg.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://tig.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cih.shanyushiyangtech.top

[G16] 对象转数组 / 字典
来源：http://bvy.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tar.jlsjyb.cn

PHP:  get_object_vars($obj);
来源：http://qki.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://ofq.fengsongda.top

TS:   Object.entries(obj)
来源：http://zje.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tqd.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tsc.yanxiufei.cn

Ruby: obj.instance_variables
来源：http://kdl.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://lvq.guannengcc.top

================================================================================
来源：http://fdm.ehwqpu.com

H. 异常与错误处理
来源：http://rue.chenjidiqi.icu

================================================================================
来源：http://dkk.0kj1m.cn

[H01] try / catch 基础
来源：http://kiv.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ypy.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sjw.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fma.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://etn.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rug.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://idi.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zhm.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yoy.yj20258.top

[H02] finally / ensure 收尾
来源：http://xmv.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://raj.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lea.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eet.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cvd.fehbvm.com


<!-- 参考信息 -->