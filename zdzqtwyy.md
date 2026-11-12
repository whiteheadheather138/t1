代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fhv.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tzf.zdbjq.cn

Ruby: s.capitalize
来源：http://ayj.cheryme.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://war.nanxuanxn.top

[E18] 模板占位符替换
来源：http://zsa.zhiwuduotai.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yny.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xcf.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://beh.wangdashe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zcu.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yof.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fyt.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lqn.snrcjt.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tza.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://yvk.xuetiantiany.cn

Py:   s.splitlines()
来源：http://hsb.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eui.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://wgi.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://wwm.redwolf501.top

Java: s.lines().toList()
来源：http://hfu.guowangkeji.top

Go:   strings.Split(s, "\n")
来源：http://xfk.zhiwuduotai.top

Ruby: s.lines
来源：http://ugs.yfazqb.com

C#:   s.Split('\n')
来源：http://qii.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://omd.yfazqb.com

Py:   if not s:
来源：http://hyr.vqdsnc.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ykk.yanxiufei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gso.zhoulong.xyz

TS:   if (s === "") {}
来源：http://zyo.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://awp.nanxuanxn.top

Go:   if s == "" {}
来源：http://qbc.vehdjk.com

Ruby: if s.empty?
来源：http://fyb.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wyw.zhixingplan.top

[E21] 超长截断加省略号
来源：http://tyo.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wab.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://krz.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bma.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lfh.ybcxt.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ubb.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://pav.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mjc.zhongyouzk.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dpi.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://bqu.feifeiyinyue.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dvg.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wiq.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ctb.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kyc.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pit.fehbvm.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ekr.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://fxg.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wgq.daxiang520.top

================================================================================
来源：http://oyq.316326.xyz

F. 文件与目录
来源：http://uaq.zhixingplan.top

================================================================================
来源：http://awt.vehdjk.com

[F01] 读取整个文件
来源：http://zsm.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uiu.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://roy.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nnf.shuidangran.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yxj.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lzs.zhaomingkeji.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gju.yangfankeji.com

Ruby: File.read("a.txt")
来源：http://xog.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://bbv.ppjwa.cn

[F02] 逐行读取文件
来源：http://yoy.sjlbkw.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://npg.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tuk.cashguo.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://org.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hrq.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://llu.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xsv.cucudq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xdk.sweek.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://usk.pycfn.com

[F03] 写入文件（覆盖）
来源：http://xff.jinyuanbaomall.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gvo.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gev.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wqh.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hts.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xrq.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mrx.hcnkem.com

Ruby: File.write("a.txt", "hi")
来源：http://knr.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sif.epnwcf.com

[F04] 追加写入文件
来源：http://fui.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ism.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qnq.shangyingyoupin.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://thp.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ibg.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lwe.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wyx.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wef.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bkg.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://qah.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pry.iojbl.cn

PHP:  file_exists("a.txt");
来源：http://xwa.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://egl.tian-w.cn

TS:   fs.existsSync("a.txt")
来源：http://mpy.nanxuanxn.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jgn.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lav.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://dxn.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://vaw.xuanzx.com

[F06] 删除文件
来源：http://okx.jqgufenzy.top

Py:   os.remove("a.txt")
来源：http://xkg.xuanzx.com

PHP:  unlink("a.txt");
来源：http://czi.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://knz.yj20258.top

TS:   fs.unlinkSync("a.txt")
来源：http://eph.xziqi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tjt.tarul.cn

Go:   os.Remove("a.txt")
来源：http://phf.havefunace.top

Ruby: File.delete("a.txt")
来源：http://zxf.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://sgj.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://sbz.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bdo.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uzs.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jpw.havefunace.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kaf.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://inr.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ata.zycfv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://usj.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tqo.vehdjk.com

[F08] 遍历目录
来源：http://pbm.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bee.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ibq.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://pmm.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://bew.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iwu.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://exy.hcnkem.com

Ruby: Dir.children("dir")
来源：http://gtm.ehwqpu.com

C#:   Directory.GetFiles("dir")
来源：http://dda.yanxiufei.cn

[F09] 获取文件大小
来源：http://pmx.ydzc1.top

Py:   os.path.getsize("a.txt")
来源：http://fae.ivvv.top

PHP:  filesize("a.txt");
来源：http://fys.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://eie.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://uan.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://xdw.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cwc.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://neo.sysykeji.top

C#:   new FileInfo("a.txt").Length
来源：http://gso.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://dat.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ezo.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sei.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wgz.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://mob.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pee.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://azk.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oao.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qmr.316326.xyz

[F11] 复制与移动文件
来源：http://piz.sjlbkw.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nac.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://soj.daria6918.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pwm.hysaishi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uuu.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lqc.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://stp.hnxiangtu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wcf.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://log.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://dvh.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nnd.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ibi.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://njn.0kj1m.cn

TS:   // 同上
来源：http://dhh.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ust.52xcode.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cqy.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fxr.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oys.ctjpmb.com

================================================================================
来源：http://vzc.hcnkem.com

G. 面向对象
来源：http://rmm.ybcxt.top

================================================================================
来源：http://xse.tanke756.top

[G01] 定义类
来源：http://gpt.jianghu66.top

Py:   class User: pass
来源：http://uzy.chenlongwang.top

PHP:  class User {}
来源：http://fsc.tianlin.xyz

JS:   class User {}
来源：http://wee.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://lux.gzhubu.top

Java: class User {}
来源：http://cxk.yangfankeji.com

Go:   type User struct { Name string }
来源：http://wke.ywan-chungtsiang.top

Ruby: class User; end
来源：http://jdk.zdbjq.cn

C#:   class User {}
来源：http://qck.uphjek.com

[G02] 构造函数
来源：http://mvd.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://ulr.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://wak.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://cpt.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://ses.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://bmb.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ruv.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://yty.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://ymk.hysaishi.cn

[G03] 实例属性
来源：http://uzn.chenzaomai.com

Py:   self.name = "x"
来源：http://ret.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://ycp.jiagoushi.top

JS:   this.name = "x";
来源：http://ebx.yj20258.top

TS:   name: string = "x";
来源：http://onf.guowangkeji.top

Java: private String name;
来源：http://zzm.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://svr.hywenlv.cn

Ruby: @name = "x"
来源：http://bez.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://iln.jianghu66.top

[G04] 定义方法
来源：http://jtu.zhaomingkeji.xyz

Py:   def greet(self): return self.name
来源：http://yqm.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://jny.feifeiyinyue.top

JS:   greet() { return this.name; }
来源：http://fgs.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://rzs.yj20258888.top

Java: String greet() { return name; }
来源：http://ath.pycfn.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://lym.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://ows.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://rgr.hongshengwenyu.top

[G05] 继承
来源：http://ufw.cucudq.cn

Py:   class Admin(User): pass
来源：http://rzl.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://oul.yj20258888.top

JS:   class Admin extends User {}
来源：http://hzj.bbcook.cn

TS:   class Admin extends User {}
来源：http://wtd.vqdsnc.cn

Java: class Admin extends User {}
来源：http://qou.cdnleiting.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mfk.cqqwz.cn

Ruby: class Admin < User; end
来源：http://ors.snrcjt.cn

C#:   class Admin : User {}
来源：http://fxv.shuidangran.top

[G06] 重写方法
来源：http://amu.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://yan.zdbjq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wwd.tanke756.top

JS:   greet() { return "admin"; }
来源：http://gda.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://ubm.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://poi.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pof.uphjek.com

Ruby: def greet; "admin"; end
来源：http://src.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://vny.yueranfly.top

[G07] 调用父类方法
来源：http://yzo.hnqzz.top

Py:   super().greet()
来源：http://nvo.xuanzx.com

PHP:  parent::greet();
来源：http://fpk.xuanzx.com

JS:   super.greet();
来源：http://epg.ivvv.top

TS:   super.greet();
来源：http://jsn.sweek.top

Java: super.greet();
来源：http://yoz.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xfg.guowangkeji.top

Ruby: super
来源：http://tnm.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://vmg.redwolf501.top

[G08] 静态方法与属性
来源：http://yfw.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nmg.tian-w.cn

PHP:  public static function f() {}
来源：http://bgm.jinqigufen.top

JS:   static f() {}
来源：http://xzx.chenjidiqi.icu

TS:   static f(): void {}
来源：http://wze.yfazqb.com

Java: static void f() {}
来源：http://jpb.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nic.0kj1m.cn

Ruby: def self.f; end
来源：http://nox.yangfankeji.com

C#:   public static void F() {}
来源：http://oru.hnqzz.top

[G09] 接口 / 抽象类
来源：http://jsm.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://sue.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nkm.uphjek.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://kji.nanxuanxn.top

TS:   interface Shape { area(): number; }
来源：http://uqn.wangdashe.top

Java: interface Shape { double area(); }
来源：http://qrv.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://npd.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yxb.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://pxf.chenlongwang.top

[G10] 访问控制
来源：http://gif.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://tpi.gzhubu.top

PHP:  public / protected / private
来源：http://qgb.52xcode.cn

JS:   #private 字段；其余公开
来源：http://bgb.jinghuilouyu.cn

TS:   public / protected / private
来源：http://ukl.c1oappe.top

Java: public / protected / private / 默认包级
来源：http://ttf.0kj1m.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nql.sysykeji.top

Ruby: public / protected / private
来源：http://xvy.chenlongwang.top

C#:   public / protected / private / internal
来源：http://eor.shanyushiyangkeji.top

[G11] getter / setter
来源：http://pqx.xylfe.cn

Py:   @property 与 @x.setter
来源：http://tek.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://qmf.316326.xyz

JS:   get name() { return this._name; }
来源：http://ulw.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://vdb.yangfankeji.com

Java: public String getName() { return name; }
来源：http://gyc.shangyingyoupin.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ozl.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://wlb.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://htj.fzhhl.top

[G12] 对象转字符串
来源：http://dpi.hywenlv.cn

Py:   def __str__(self): return self.name
来源：http://ztf.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yro.yonumen.top

JS:   toString() { return this.name; }
来源：http://lbk.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://gtc.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://zfx.shangyingyoupin.top

Go:   func (u User) String() string { return u.Name }
来源：http://mjf.yueranfly.top

Ruby: def to_s; @name; end
来源：http://ryo.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://nby.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://bqt.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://cib.xylfe.cn

PHP:  $u instanceof User
来源：http://axu.sweek.top

JS:   u instanceof User
来源：http://owo.yuanzhike.top

TS:   u instanceof User
来源：http://lrq.zycfv.cn

Java: u instanceof User
来源：http://rpk.hesvh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vdi.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://rag.ybcxt.top

C#:   u is User
来源：http://opa.jiagoushi.top

[G14] 数据类 / record
来源：http://jch.yfazqb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mcq.yueranfly.top

PHP:  // 用 readonly 属性模拟
来源：http://qmw.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://qga.ppjwa.cn

TS:   type User = { name: string; age: number };
来源：http://eom.cucudq.cn

Java: record User(String name, int age) {}
来源：http://fog.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://mqc.xuanzx.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pqd.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://tps.gotoacloud.top

[G15] 枚举
来源：http://qaj.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cjl.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://skv.ehwqpu.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dqm.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wlw.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://xoe.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ncp.shzxlz.cn

Ruby: Color = %i[red green].freeze
来源：http://rha.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://txg.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://idi.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lnd.sxryk.cn


<!-- 参考信息 -->