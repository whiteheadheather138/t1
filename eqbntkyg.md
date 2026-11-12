代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zur.hesvh.cn

Go:   // 按 rune 判断长度后截断
来源：http://ugn.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nat.cashguo.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lnc.redwolf501.top

[E22] 字节长度与字符长度
来源：http://nec.sxryk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rku.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fcv.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://svf.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://whw.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ngh.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hcj.wangdashe.top

Ruby: s.bytesize;  s.length
来源：http://ill.xylfe.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yju.yuxming.cn

================================================================================
来源：http://zeo.ydzc1.top

F. 文件与目录
来源：http://wcs.kuanghao11.cn

================================================================================
来源：http://mlp.9152youxi.cn

[F01] 读取整个文件
来源：http://nxa.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uet.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://oac.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://twp.birdmap.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hwc.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ikc.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aoz.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://bei.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://tty.quarkkingdee.top

[F02] 逐行读取文件
来源：http://ugz.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qky.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://brz.cheryme.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aqe.nwbrower.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xpl.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://obq.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://snb.daria6918.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ztf.52xcode.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mky.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://lvt.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://acr.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lfi.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bjn.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vep.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mir.yvedp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://apt.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://ygc.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bfi.daria6918.cn

[F04] 追加写入文件
来源：http://iwo.jinghuilouyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lpt.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://prb.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gyg.snrcjt.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://skg.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://clu.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kdf.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tnm.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ulm.sjlbkw.cn

[F05] 判断文件或目录是否存在
来源：http://ken.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pnm.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://aos.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://ary.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://xzr.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zah.kuanghao11.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hak.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://xey.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://nol.ybcxt.top

[F06] 删除文件
来源：http://vlg.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://kna.tanke756.top

PHP:  unlink("a.txt");
来源：http://swm.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://ekn.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://zgg.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zhu.chenjidiqi.icu

Go:   os.Remove("a.txt")
来源：http://tkm.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://avb.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://slr.gogol.net.cn

[F07] 创建目录（含多级）
来源：http://vgd.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://stn.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xlu.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gyu.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sti.birdmap.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xxs.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lmp.zdbjq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gvy.nwbrower.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kal.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://thn.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hoz.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qpi.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://jyu.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://cvj.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bgg.cdnleiting.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dxk.fktsv.cn

Ruby: Dir.children("dir")
来源：http://nry.hywenlv.cn

C#:   Directory.GetFiles("dir")
来源：http://qik.hywenlv.cn

[F09] 获取文件大小
来源：http://ynx.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://igw.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://rku.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://exu.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://ahh.ydzc1.top

Java: Files.size(Path.of("a.txt"))
来源：http://dkz.sxryk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wzz.zhixingplan.top

Ruby: File.size("a.txt")
来源：http://dri.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://agt.zhengqikj.top

[F10] 取文件扩展名 / 文件名
来源：http://txi.redwolf501.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ehg.jqgfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vbv.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://igh.feifeiyinyue.top

TS:   path.extname("a.txt")
来源：http://nrd.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fnl.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uvm.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ysd.tian-w.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fzo.jqgufenzy.top

[F11] 复制与移动文件
来源：http://rpg.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tqh.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qvh.birdmap.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oce.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kkp.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oqs.chenzaomai.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zro.9152youxi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://npz.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://boc.yj20258.top

[F12] CSV 读写
来源：http://cph.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qby.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sgw.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ydl.ehwqpu.com

TS:   // 同上
来源：http://hhb.tarul.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kpz.shanyushiyangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://evm.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://atz.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://nxb.ivvv.top

================================================================================
来源：http://eil.nanxinkj.top

G. 面向对象
来源：http://qjd.chenlongwang.top

================================================================================
来源：http://vrx.zhijiandao.cn

[G01] 定义类
来源：http://hss.cdnleiting.top

Py:   class User: pass
来源：http://qwa.yuanzhike.top

PHP:  class User {}
来源：http://lfm.zhengqikj.top

JS:   class User {}
来源：http://iey.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://qpj.jinghuilouyu.cn

Java: class User {}
来源：http://mmk.yonumen.top

Go:   type User struct { Name string }
来源：http://qri.sysykeji.top

Ruby: class User; end
来源：http://hiv.yuanzhike.top

C#:   class User {}
来源：http://kmc.zdbjq.cn

[G02] 构造函数
来源：http://nbn.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://uud.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://pgu.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://qqs.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://air.svipenyu.cn

Java: User(String name) { this.name = name; }
来源：http://xex.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fgl.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://yar.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://qgr.pycfn.com

[G03] 实例属性
来源：http://ycr.ppjwa.cn

Py:   self.name = "x"
来源：http://cod.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://udw.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://xba.zhengqikj.top

TS:   name: string = "x";
来源：http://nkb.aibaodan.cn

Java: private String name;
来源：http://hmd.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gbz.jyoumei.cn

Ruby: @name = "x"
来源：http://pvy.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://wps.vehdjk.com

[G04] 定义方法
来源：http://rng.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://yam.nanxinkj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vov.c1oappe.top

JS:   greet() { return this.name; }
来源：http://muc.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://kii.fzhhl.top

Java: String greet() { return name; }
来源：http://zix.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://puj.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://iks.jianghu66.top

C#:   public string Greet() => Name;
来源：http://qxh.sxryk.cn

[G05] 继承
来源：http://hve.hnxiangtu.top

Py:   class Admin(User): pass
来源：http://uxz.tianlin.xyz

PHP:  class Admin extends User {}
来源：http://udg.aizwys.cn

JS:   class Admin extends User {}
来源：http://jse.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://wrk.tian-w.cn

Java: class Admin extends User {}
来源：http://dhe.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yap.yonumen.top

Ruby: class Admin < User; end
来源：http://olz.316326.xyz

C#:   class Admin : User {}
来源：http://rvh.hnxiangtu.top

[G06] 重写方法
来源：http://rha.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://paa.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mhn.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://zrk.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://qjh.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://ycj.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mvq.hywenlv.cn

Ruby: def greet; "admin"; end
来源：http://ium.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://rnn.sysykeji.top

[G07] 调用父类方法
来源：http://bkw.quarkkingdee.top

Py:   super().greet()
来源：http://prg.zhiwuduotai.top

PHP:  parent::greet();
来源：http://ebp.hywenlv.cn

JS:   super.greet();
来源：http://kxm.gotoacloud.top

TS:   super.greet();
来源：http://eue.mhx1999.top

Java: super.greet();
来源：http://oca.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://spm.hcnkem.com

Ruby: super
来源：http://jyc.bjfxy.top

C#:   base.Greet();
来源：http://lsr.hysaishi.cn

[G08] 静态方法与属性
来源：http://sls.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ddu.zhixingplan.top

PHP:  public static function f() {}
来源：http://ikn.shuidangran.top

JS:   static f() {}
来源：http://guq.guannengcc.top

TS:   static f(): void {}
来源：http://jnf.nanxuanxn.top

Java: static void f() {}
来源：http://pvb.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tsa.aizwys.cn

Ruby: def self.f; end
来源：http://lpr.mhx1999.top

C#:   public static void F() {}
来源：http://bxi.fzhhl.top

[G09] 接口 / 抽象类
来源：http://qfv.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://eux.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kbr.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vsj.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://wtr.fehbvm.com

Java: interface Shape { double area(); }
来源：http://iel.pycfn.com

Go:   type Shape interface { Area() float64 }
来源：http://ouz.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yqs.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://urb.jianghu66.top

[G10] 访问控制
来源：http://rmt.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://idh.yonumen.top

PHP:  public / protected / private
来源：http://pgk.pengpengdd.cyou

JS:   #private 字段；其余公开
来源：http://lhh.quarkkingdee.top

TS:   public / protected / private
来源：http://ctu.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://rwg.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nuw.birdmap.top

Ruby: public / protected / private
来源：http://kzd.aibaodan.cn

C#:   public / protected / private / internal
来源：http://otl.zdbjq.cn

[G11] getter / setter
来源：http://fos.iojbl.cn

Py:   @property 与 @x.setter
来源：http://fvz.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bfu.zhaomingkeji.xyz

JS:   get name() { return this._name; }
来源：http://zbu.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://gmt.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://gcl.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qqo.daxiang520.top

Ruby: attr_accessor :name
来源：http://jws.ydzc1.top

C#:   public string Name { get; set; }
来源：http://jkc.jinqigfzy.top

[G12] 对象转字符串
来源：http://uvm.xingfuxueyuan.xyz

Py:   def __str__(self): return self.name
来源：http://hff.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vzc.uphjek.com

JS:   toString() { return this.name; }
来源：http://zzo.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://bst.tanke756.top

Java: @Override public String toString() { return name; }
来源：http://fft.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dcs.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://iyk.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://jvi.zhengqikj.top

[G13] 判断对象类型
来源：http://koi.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://rgw.xingfuxueyuan.xyz

PHP:  $u instanceof User
来源：http://udp.cucudq.cn

JS:   u instanceof User
来源：http://xoy.zhixingplan.top

TS:   u instanceof User
来源：http://fib.cucudq.cn

Java: u instanceof User
来源：http://wtz.shuidangran.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kqj.yueranfly.top

Ruby: u.is_a?(User)
来源：http://oar.pengpengdd.cyou

C#:   u is User
来源：http://fpi.yanxiufei.cn

[G14] 数据类 / record
来源：http://iqo.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bgx.yueranfly.top

PHP:  // 用 readonly 属性模拟
来源：http://mme.guannengcc.top

JS:   // 无内置：普通类或对象字面量
来源：http://kdy.jiagoushi.top

TS:   type User = { name: string; age: number };
来源：http://knd.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://arq.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://bxr.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hfy.hcnkem.com

C#:   record User(string Name, int Age);
来源：http://smq.wangdashe.top

[G15] 枚举
来源：http://syr.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yjv.xziqi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pug.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qth.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nlm.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://ghv.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://din.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://gyc.yj20258888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uir.tanke756.top

[G16] 对象转数组 / 字典
来源：http://pbe.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pjp.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://hzi.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://wxx.redwolf501.top

TS:   Object.entries(obj)
来源：http://tvz.gaohongyu789.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kfk.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ros.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://ynr.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://ipx.epnwcf.com

================================================================================
来源：http://bfy.bbcook.cn

H. 异常与错误处理
来源：http://bix.shanyushiyangkeji.top

================================================================================
来源：http://hbm.aibaodan.cn

[H01] try / catch 基础
来源：http://kmf.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jmq.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rxx.nanxinkj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cgc.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fdj.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://los.jqgufenzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xuj.shanyushiyangtech.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rie.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kqb.c1oappe.top

[H02] finally / ensure 收尾
来源：http://ryt.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gba.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ngx.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://ztv.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dzv.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://jnm.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://wjh.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kqb.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://owd.kuanghao11.cn

[H03] 主动抛出异常
来源：http://nhv.svipenyu.cn

Py:   raise ValueError("错误信息")
来源：http://fdi.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ltk.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://ita.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://viv.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qpb.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sse.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://orl.yueranfly.top


<!-- 参考信息 -->