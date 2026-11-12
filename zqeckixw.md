代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kqb.sweek.top

[E19] 多行文本按行拆分
来源：http://muv.jyoumei.cn

Py:   s.splitlines()
来源：http://otm.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wzx.sweek.top

JS:   s.split(/\r?\n/)
来源：http://hzf.shangyingyoupin.top

TS:   s.split(/\r?\n/)
来源：http://qps.52xcode.cn

Java: s.lines().toList()
来源：http://yom.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://sjj.sjlbkw.cn

Ruby: s.lines
来源：http://cnp.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://oer.52xcode.cn

[E20] 判断字符串是否为空
来源：http://odt.yuanzhike.top

Py:   if not s:
来源：http://xep.jiagoushi.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tnh.hnqzz.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yaq.xuanzx.com

TS:   if (s === "") {}
来源：http://mds.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://fwy.yuanzhike.top

Go:   if s == "" {}
来源：http://vkl.mhx1999.top

Ruby: if s.empty?
来源：http://nya.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://son.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://qtw.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lyz.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zgq.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jth.zhixingplan.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kuk.hnqzz.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jwe.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://eay.bbcook.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sok.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://szf.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://zkq.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://igi.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ask.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ghw.c1oappe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vyf.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uov.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bts.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://pug.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tja.dashuyun.cn

================================================================================
来源：http://mgd.nwbrower.top

F. 文件与目录
来源：http://qew.birdmap.top

================================================================================
来源：http://acc.yueranfly.top

[F01] 读取整个文件
来源：http://jcw.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mvs.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://ojr.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ohl.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://juh.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iyy.hysaishi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://upf.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://rqn.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://crw.shangyingyoupin.top

[F02] 逐行读取文件
来源：http://irv.9152youxi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ouz.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://coe.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vhh.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yyl.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bnu.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tfh.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ekr.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vcw.0kj1m.cn

[F03] 写入文件（覆盖）
来源：http://ofn.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lbw.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tjj.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dpb.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yce.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://asj.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rkw.jlsjyb.cn

Ruby: File.write("a.txt", "hi")
来源：http://tdt.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cga.sxryk.cn

[F04] 追加写入文件
来源：http://jyd.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qij.ehwqpu.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ytk.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eiw.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qce.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dba.sweek.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mtq.iojbl.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pmk.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://imp.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://kqq.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://voz.yongpay.top

PHP:  file_exists("a.txt");
来源：http://rvx.fengsongda.top

JS:   fs.existsSync("a.txt")
来源：http://yzf.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://hco.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xfr.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://exr.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://stv.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://nah.sjlbkw.cn

[F06] 删除文件
来源：http://fpa.hysaishi.cn

Py:   os.remove("a.txt")
来源：http://gss.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://ezl.jinqigufen.top

JS:   fs.unlinkSync("a.txt")
来源：http://avt.nanxuanxn.top

TS:   fs.unlinkSync("a.txt")
来源：http://jop.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cvt.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://kca.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://teb.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://htj.jinqigufen.top

[F07] 创建目录（含多级）
来源：http://jpy.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lcw.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qtx.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tva.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qzw.shangyingyoupin.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sfw.c1oappe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gbh.daria6918.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cfv.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oyv.cdnleiting.top

[F08] 遍历目录
来源：http://emi.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fkg.havefunace.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ibb.yfazqb.com

JS:   fs.readdirSync("dir")
来源：http://iya.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://ftx.sjlbkw.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vvi.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gle.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://hea.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://xnu.smart0.xyz

[F09] 获取文件大小
来源：http://nkn.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://nrj.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://hcm.andypj.xyz

JS:   fs.statSync("a.txt").size
来源：http://zjk.cashguo.top

TS:   fs.statSync("a.txt").size
来源：http://nyj.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://vsq.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lho.guannengcc.top

Ruby: File.size("a.txt")
来源：http://jlv.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://hee.kuanghao11.cn

[F10] 取文件扩展名 / 文件名
来源：http://hoa.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://odc.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bsj.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qss.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://bvv.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fab.cashguo.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oer.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ahm.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rhy.zdbjq.cn

[F11] 复制与移动文件
来源：http://ccc.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xuh.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jvh.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gnr.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rla.smart0.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mub.dashuyun.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tgy.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jpf.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nlv.havefunace.top

[F12] CSV 读写
来源：http://yhh.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hax.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bop.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dth.shanyushiyangkeji.top

TS:   // 同上
来源：http://eji.kuanghao11.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wce.yj20258888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kxi.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pro.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rpk.tian-w.cn

================================================================================
来源：http://wxh.shanyushiyangkeji.top

G. 面向对象
来源：http://mwy.shangyingyoupin.top

================================================================================
来源：http://nuq.fengsongda.top

[G01] 定义类
来源：http://coi.hfpthk.cn

Py:   class User: pass
来源：http://loo.jiagoushi.top

PHP:  class User {}
来源：http://hwf.cheryme.top

JS:   class User {}
来源：http://olh.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://lgn.yuanzhike.top

Java: class User {}
来源：http://tvp.cqqwz.cn

Go:   type User struct { Name string }
来源：http://rob.zhaomingkeji.xyz

Ruby: class User; end
来源：http://oho.sysykeji.top

C#:   class User {}
来源：http://xao.zhengqikj.top

[G02] 构造函数
来源：http://zxh.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://chx.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://pbw.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://qty.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://hzo.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://llc.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eus.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://www.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://dva.jinqigfzy.top

[G03] 实例属性
来源：http://bgs.ehwqpu.com

Py:   self.name = "x"
来源：http://iik.fengsongda.top

PHP:  public string $name = "x";
来源：http://xae.daxiang520.top

JS:   this.name = "x";
来源：http://umg.daxiang520.top

TS:   name: string = "x";
来源：http://eer.svipenyu.cn

Java: private String name;
来源：http://qqf.zdqjudy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wjh.hnqzz.top

Ruby: @name = "x"
来源：http://ccl.ctjpmb.com

C#:   public string Name { get; set; } = "x";
来源：http://mia.gaohongyu789.top

[G04] 定义方法
来源：http://uiv.fktsv.cn

Py:   def greet(self): return self.name
来源：http://xkj.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://svx.daria6918.cn

JS:   greet() { return this.name; }
来源：http://qul.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://lud.dianchejie.cn

Java: String greet() { return name; }
来源：http://noz.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xfn.hesvh.cn

Ruby: def greet; @name; end
来源：http://zcp.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://bis.snrcjt.cn

[G05] 继承
来源：http://tmp.sysykeji.top

Py:   class Admin(User): pass
来源：http://dxd.c1oappe.top

PHP:  class Admin extends User {}
来源：http://prx.jinqigufen.top

JS:   class Admin extends User {}
来源：http://yto.jqgfzy.top

TS:   class Admin extends User {}
来源：http://lzn.haohaochexian.top

Java: class Admin extends User {}
来源：http://mrn.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xrq.gzhubu.top

Ruby: class Admin < User; end
来源：http://nkk.sjlbkw.cn

C#:   class Admin : User {}
来源：http://ggf.yonumen.top

[G06] 重写方法
来源：http://jbi.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://csy.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wxd.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://fdy.sufxvd.cn

TS:   greet(): string { return "admin"; }
来源：http://pdl.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://tly.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vba.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://wuf.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://thc.uphjek.com

[G07] 调用父类方法
来源：http://ymc.dianchejie.cn

Py:   super().greet()
来源：http://hrc.fktsv.cn

PHP:  parent::greet();
来源：http://vpu.jianghu66.top

JS:   super.greet();
来源：http://vrs.hesvh.cn

TS:   super.greet();
来源：http://yji.epnwcf.com

Java: super.greet();
来源：http://scu.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mmi.hongshengwenyu.top

Ruby: super
来源：http://clz.hysaishi.cn

C#:   base.Greet();
来源：http://jac.tian-w.cn

[G08] 静态方法与属性
来源：http://mri.ydzc1.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vcz.ydzc1.top

PHP:  public static function f() {}
来源：http://yxm.yvedp.cn

JS:   static f() {}
来源：http://zoa.hnxiangtu.top

TS:   static f(): void {}
来源：http://chl.guannengcc.top

Java: static void f() {}
来源：http://ifx.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wdy.redwolf501.top

Ruby: def self.f; end
来源：http://tap.ctjpmb.com

C#:   public static void F() {}
来源：http://pgm.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://lrw.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://bfa.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://wsq.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dyr.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://ysx.52xcode.cn

Java: interface Shape { double area(); }
来源：http://uba.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://wnu.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dmj.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://lbk.vehdjk.com

[G10] 访问控制
来源：http://idc.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://hbt.shangyingyoupin.top

PHP:  public / protected / private
来源：http://mdm.ppjwa.cn

JS:   #private 字段；其余公开
来源：http://cst.havefunace.top

TS:   public / protected / private
来源：http://iiv.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://ryh.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://kva.jyoumei.cn

Ruby: public / protected / private
来源：http://ibs.yj20258888.top

C#:   public / protected / private / internal
来源：http://fgn.xylfe.cn

[G11] getter / setter
来源：http://zwu.guowangkeji.top

Py:   @property 与 @x.setter
来源：http://rli.jqgufenzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://toz.yj20258.top

JS:   get name() { return this._name; }
来源：http://pgl.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://nge.cucudq.cn

Java: public String getName() { return name; }
来源：http://gdv.jinqigfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bwz.c1oappe.top

Ruby: attr_accessor :name
来源：http://nkz.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://ric.wangdashe.top

[G12] 对象转字符串
来源：http://ktn.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://eri.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hyw.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://uin.zhixingplan.top

TS:   toString(): string { return this.name; }
来源：http://psc.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://fxn.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://ypu.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://cdt.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://xqa.chenjidiqi.icu

[G13] 判断对象类型
来源：http://mgk.mhx1999.top

Py:   isinstance(u, User)
来源：http://eoh.tian-w.cn

PHP:  $u instanceof User
来源：http://ulc.zhixingplan.top

JS:   u instanceof User
来源：http://fju.cucudq.cn

TS:   u instanceof User
来源：http://mhi.kuanghao11.cn

Java: u instanceof User
来源：http://exs.zycfv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zvi.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://kdf.hnxiangtu.top

C#:   u is User
来源：http://vhx.guowangkeji.top

[G14] 数据类 / record
来源：http://jgc.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nvr.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://jvs.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://xoa.yanxiufei.cn

TS:   type User = { name: string; age: number };
来源：http://vvl.cheryme.top

Java: record User(String name, int age) {}
来源：http://qgy.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://pri.aizwys.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hpf.yj202588.top

C#:   record User(string Name, int Age);
来源：http://iwv.yuanzhike.top

[G15] 枚举
来源：http://zbi.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bte.sjlbkw.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zez.jqgufenzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ncw.yanxiufei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ikw.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://zhw.hcnkem.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ins.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://byu.hesvh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hcw.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://tac.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gzy.xinyue.icu

PHP:  get_object_vars($obj);
来源：http://vxw.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://rni.yuanzhike.top

TS:   Object.entries(obj)
来源：http://azt.52xcode.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oap.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vfj.hcnkem.com

Ruby: obj.instance_variables
来源：http://qcj.redwolf501.top

C#:   // 用反射或 System.Text.Json
来源：http://wgf.shangyingyoupin.top

================================================================================
来源：http://ybr.yangfankeji.com

H. 异常与错误处理
来源：http://eod.xuanzx.com

================================================================================
来源：http://iuh.hysaishi.cn

[H01] try / catch 基础
来源：http://laj.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pxs.jlsjyb.cn


<!-- 参考信息 -->