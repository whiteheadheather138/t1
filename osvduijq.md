代发 wailian999

Ruby: s.lines
来源：http://fbq.cheryme.top

C#:   s.Split('\n')
来源：http://yzr.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://zys.hywenlv.cn

Py:   if not s:
来源：http://cbr.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ghm.xziqi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lcj.xingfuxueyuan.xyz

TS:   if (s === "") {}
来源：http://beo.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://pnt.jqgfzy.top

Go:   if s == "" {}
来源：http://zkw.bbcook.cn

Ruby: if s.empty?
来源：http://png.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xmu.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://pcf.zhixingplan.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nto.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://onc.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qjh.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hyw.hesvh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dpl.zhiwuduotai.top

Go:   // 按 rune 判断长度后截断
来源：http://fsc.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ier.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ejd.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://bpy.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zsb.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bpz.wangshuangyany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lls.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uao.ivvv.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tzj.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tni.jinqigfzy.top

Ruby: s.bytesize;  s.length
来源：http://gop.zycfv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tmj.haohaochexian.top

================================================================================
来源：http://box.guannengcc.top

F. 文件与目录
来源：http://mig.wangshuangyany.cn

================================================================================
来源：http://llj.bbcook.cn

[F01] 读取整个文件
来源：http://hmc.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tcz.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://yto.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://abz.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oob.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://jyk.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://txw.tian-w.cn

Ruby: File.read("a.txt")
来源：http://tvf.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://sbh.quarkkingdee.top

[F02] 逐行读取文件
来源：http://asd.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jmt.cucudq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://akx.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kgn.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mxb.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wqh.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aju.yueranfly.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wjl.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nxq.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://nje.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lzf.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://agg.yangfankeji.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mht.birdmap.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://whx.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jhg.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://szi.yangfankeji.com

Ruby: File.write("a.txt", "hi")
来源：http://tiw.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ixl.chenjidiqi.icu

[F04] 追加写入文件
来源：http://rdo.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sld.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wdk.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://twd.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://igu.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zxh.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hrq.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jtk.daria6918.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tej.aizwys.cn

[F05] 判断文件或目录是否存在
来源：http://tgc.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vek.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://twd.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://wbs.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://qro.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jmb.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://inp.cucudq.cn

Ruby: File.exist?("a.txt")
来源：http://zhn.zhoulong.xyz

C#:   File.Exists("a.txt")
来源：http://ycg.fzhhl.top

[F06] 删除文件
来源：http://fyr.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://jnt.yj20258.top

PHP:  unlink("a.txt");
来源：http://wpc.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://yho.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ang.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kxo.ybcxt.top

Go:   os.Remove("a.txt")
来源：http://qeo.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://lwg.fzhhl.top

C#:   File.Delete("a.txt");
来源：http://qfr.ivvv.top

[F07] 创建目录（含多级）
来源：http://xeb.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ipv.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://etg.pycfn.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ont.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cgh.guannengcc.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wvi.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nol.wangdashe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nyy.meibo888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://voj.cheryme.top

[F08] 遍历目录
来源：http://zoy.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://pao.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hmr.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://are.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://kde.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rvc.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://rgu.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://gfp.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://wtt.jyoumei.cn

[F09] 获取文件大小
来源：http://iil.andypj.xyz

Py:   os.path.getsize("a.txt")
来源：http://dgg.bjfxy.top

PHP:  filesize("a.txt");
来源：http://xkh.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://slt.hongshengwenyu.top

TS:   fs.statSync("a.txt").size
来源：http://vcf.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sxj.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://asd.zhoulong.xyz

Ruby: File.size("a.txt")
来源：http://snk.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://bsx.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://auu.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kls.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://llu.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xur.vehdjk.com

TS:   path.extname("a.txt")
来源：http://zze.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bwq.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qaf.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lwc.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rhg.52xcode.cn

[F11] 复制与移动文件
来源：http://jgn.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://llc.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://alw.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xzn.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eec.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tyf.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vwc.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cfr.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kqn.dianchejie.cn

[F12] CSV 读写
来源：http://zul.jlsjyb.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tjt.zdqjudy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ezr.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://plz.jlsjyb.cn

TS:   // 同上
来源：http://nzw.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jsr.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kqg.sysykeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dwz.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://owq.feifeiyinyue.top

================================================================================
来源：http://wmt.kuanghao11.cn

G. 面向对象
来源：http://mgb.xylfe.cn

================================================================================
来源：http://slc.ctjpmb.com

[G01] 定义类
来源：http://cgj.sjlbkw.cn

Py:   class User: pass
来源：http://cfh.kuanghao11.cn

PHP:  class User {}
来源：http://rgr.nanxinkj.top

JS:   class User {}
来源：http://chn.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://ybs.jinqigfzy.top

Java: class User {}
来源：http://ywj.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://loi.9152youxi.cn

Ruby: class User; end
来源：http://pnz.daria6918.cn

C#:   class User {}
来源：http://emb.birdmap.top

[G02] 构造函数
来源：http://hrq.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://xkh.zhoulong.xyz

PHP:  public function __construct(public string $name) {}
来源：http://arp.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://fle.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://fbc.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://eai.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lvx.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://xkb.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://sun.svipenyu.cn

[G03] 实例属性
来源：http://sdq.aizwys.cn

Py:   self.name = "x"
来源：http://uwb.fehbvm.com

PHP:  public string $name = "x";
来源：http://txe.fzhhl.top

JS:   this.name = "x";
来源：http://cpb.smart0.xyz

TS:   name: string = "x";
来源：http://iil.ywan-chungtsiang.top

Java: private String name;
来源：http://ncs.ydjk.org.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mho.daria6918.cn

Ruby: @name = "x"
来源：http://ahn.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://sjn.jlsjyb.cn

[G04] 定义方法
来源：http://oku.ivvv.top

Py:   def greet(self): return self.name
来源：http://bej.jinghuilouyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lsq.shuidangran.top

JS:   greet() { return this.name; }
来源：http://ctw.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://det.yj20258888.top

Java: String greet() { return name; }
来源：http://qqz.xinyue.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://wkz.havefunace.top

Ruby: def greet; @name; end
来源：http://viv.fehbvm.com

C#:   public string Greet() => Name;
来源：http://axo.yj20258.top

[G05] 继承
来源：http://xxr.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://sua.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://rhz.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://ocl.guannengcc.top

TS:   class Admin extends User {}
来源：http://ghl.svipenyu.cn

Java: class Admin extends User {}
来源：http://bdz.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xtd.yj20258.top

Ruby: class Admin < User; end
来源：http://yjk.wangdashe.top

C#:   class Admin : User {}
来源：http://wyk.feifeiyinyue.top

[G06] 重写方法
来源：http://tlk.hysaishi.cn

Py:   def greet(self): return "admin"
来源：http://lld.hnqzz.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fzl.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://rec.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://xmv.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://fvd.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zci.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://ngw.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://tlj.nanxinkj.top

[G07] 调用父类方法
来源：http://pnk.ctjpmb.com

Py:   super().greet()
来源：http://ckw.iojbl.cn

PHP:  parent::greet();
来源：http://wlt.jqgfzy.top

JS:   super.greet();
来源：http://rwk.guowangkeji.top

TS:   super.greet();
来源：http://ybe.cdnleiting.top

Java: super.greet();
来源：http://txd.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hbi.fanxiaobao.xyz

Ruby: super
来源：http://nxc.snrcjt.cn

C#:   base.Greet();
来源：http://rnl.shuidangran.top

[G08] 静态方法与属性
来源：http://wbq.dashuyun.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ohh.52xcode.cn

PHP:  public static function f() {}
来源：http://jtu.ehwqpu.com

JS:   static f() {}
来源：http://pzt.nanxuanxn.top

TS:   static f(): void {}
来源：http://ozj.tianlin.xyz

Java: static void f() {}
来源：http://ism.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cnc.yongpay.top

Ruby: def self.f; end
来源：http://cjs.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://utm.nwbrower.top

[G09] 接口 / 抽象类
来源：http://agy.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://zih.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bkp.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vgg.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://awf.gotoacloud.top

Java: interface Shape { double area(); }
来源：http://due.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://kim.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cvq.cucudq.cn

C#:   interface IShape { double Area(); }
来源：http://ujy.hammf.cn

[G10] 访问控制
来源：http://yxr.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://gvf.ydzc1.top

PHP:  public / protected / private
来源：http://stj.sysykeji.top

JS:   #private 字段；其余公开
来源：http://kjl.bbcook.cn

TS:   public / protected / private
来源：http://clo.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://buw.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fcj.quarkkingdee.top

Ruby: public / protected / private
来源：http://wvd.gotoacloud.top

C#:   public / protected / private / internal
来源：http://fxy.tarul.cn

[G11] getter / setter
来源：http://zno.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://egg.316326.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://dyx.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://dol.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://zpr.sweek.top

Java: public String getName() { return name; }
来源：http://gkk.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yrv.aizwys.cn

Ruby: attr_accessor :name
来源：http://dtb.fktsv.cn

C#:   public string Name { get; set; }
来源：http://wbd.hnxiangtu.top

[G12] 对象转字符串
来源：http://kry.feifeiyinyue.top

Py:   def __str__(self): return self.name
来源：http://ptk.zhengqikj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nni.bjfxy.top

JS:   toString() { return this.name; }
来源：http://xjg.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://wrh.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://asx.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://adu.daxiang520.top

Ruby: def to_s; @name; end
来源：http://xlr.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://tup.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://rvs.havefunace.top

Py:   isinstance(u, User)
来源：http://hap.ybcxt.top

PHP:  $u instanceof User
来源：http://ggz.ctjpmb.com

JS:   u instanceof User
来源：http://wxu.yanxiufei.cn

TS:   u instanceof User
来源：http://btk.xylfe.cn

Java: u instanceof User
来源：http://vhy.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://gaj.ivvv.top

Ruby: u.is_a?(User)
来源：http://vvc.sweek.top

C#:   u is User
来源：http://jbf.ppjwa.cn

[G14] 数据类 / record
来源：http://jto.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jqb.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://rpt.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://kux.birdmap.top

TS:   type User = { name: string; age: number };
来源：http://yas.yj202588.top

Java: record User(String name, int age) {}
来源：http://efa.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://cnx.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hhv.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://wgh.0kj1m.cn

[G15] 枚举
来源：http://yfc.jinyuanbaomall.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://raf.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ubw.ywan-chungtsiang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://amb.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fsa.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://eeb.ydjk.org.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pas.hongshengwenyu.top

Ruby: Color = %i[red green].freeze
来源：http://ckf.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://foc.316326.xyz

[G16] 对象转数组 / 字典
来源：http://amg.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wny.epnwcf.com

PHP:  get_object_vars($obj);
来源：http://rlu.yuxming.cn

JS:   Object.entries(obj)
来源：http://csl.havefunace.top

TS:   Object.entries(obj)
来源：http://vaj.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rya.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wjl.snrcjt.cn

Ruby: obj.instance_variables
来源：http://chp.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://moj.andypj.xyz

================================================================================
来源：http://rjw.xuanzx.com

H. 异常与错误处理
来源：http://upy.yonumen.top

================================================================================
来源：http://srh.daria6918.cn

[H01] try / catch 基础
来源：http://svy.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gsj.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lio.zhiwuduotai.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cee.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gpa.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kuu.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ois.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bft.ydjk.org.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tkl.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://ved.hfpthk.cn


<!-- 参考信息 -->