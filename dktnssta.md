代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vlc.9152youxi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jng.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mat.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tvi.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wms.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pzy.c1oappe.top

Ruby: s.capitalize
来源：http://mtk.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tcr.hcnkem.com

[E18] 模板占位符替换
来源：http://pix.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nmx.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sbl.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://hpt.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vzm.yj20258.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zrw.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tmm.zhixingplan.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rjw.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mep.yuxming.cn

[E19] 多行文本按行拆分
来源：http://vab.meibo888.top

Py:   s.splitlines()
来源：http://mvn.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xlt.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://vhu.cdnleiting.top

TS:   s.split(/\r?\n/)
来源：http://gok.dianchejie.cn

Java: s.lines().toList()
来源：http://bja.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://vqx.cqqwz.cn

Ruby: s.lines
来源：http://ybd.andypj.xyz

C#:   s.Split('\n')
来源：http://flz.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://abc.316326.xyz

Py:   if not s:
来源：http://sxv.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iaa.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vju.ydjk.org.cn

TS:   if (s === "") {}
来源：http://mdw.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://usg.daria6918.cn

Go:   if s == "" {}
来源：http://cuv.jlsjyb.cn

Ruby: if s.empty?
来源：http://gpz.fzhhl.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dzt.shzxlz.cn

[E21] 超长截断加省略号
来源：http://ojv.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rtd.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qwf.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hbz.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vwk.zycfv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ffc.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://yjf.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oyh.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sko.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://wnw.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nbu.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pcf.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uzh.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tlu.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oap.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jjr.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://xkj.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oro.daria6918.cn

================================================================================
来源：http://aqf.xylfe.cn

F. 文件与目录
来源：http://jqb.yanxiufei.cn

================================================================================
来源：http://eht.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://lrt.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://szn.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://vus.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fkg.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ofc.chenlongwang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wmb.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kif.xingfuxueyuan.xyz

Ruby: File.read("a.txt")
来源：http://bgd.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://xxs.snrcjt.cn

[F02] 逐行读取文件
来源：http://vuo.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lem.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pea.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bdt.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://isj.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mvf.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hyk.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://htb.guowangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://utr.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://shb.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fgl.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wan.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tly.xinyue.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zcu.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://crs.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yjm.shzxlz.cn

Ruby: File.write("a.txt", "hi")
来源：http://pzz.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oml.zhixingplan.top

[F04] 追加写入文件
来源：http://pjl.jinghuilouyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mhj.gotoacloud.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mli.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://khd.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://voy.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ijs.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ncc.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hwp.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hlr.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://yah.fktsv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://znz.316326.xyz

PHP:  file_exists("a.txt");
来源：http://hvd.sweek.top

JS:   fs.existsSync("a.txt")
来源：http://ncp.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://pdc.yongpay.top

Java: Files.exists(Path.of("a.txt"))
来源：http://arm.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uqh.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://wkx.yj20258.top

C#:   File.Exists("a.txt")
来源：http://jcw.yuanzhike.top

[F06] 删除文件
来源：http://bjv.c1oappe.top

Py:   os.remove("a.txt")
来源：http://zrs.guannengcc.top

PHP:  unlink("a.txt");
来源：http://bhx.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://idr.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://zsn.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ixe.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://xko.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://ncn.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://hdn.mhx1999.top

[F07] 创建目录（含多级）
来源：http://lms.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kfr.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nah.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://win.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hoi.316326.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://swz.shangyingyoupin.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bye.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dfm.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mhx.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://dum.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://zee.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dxe.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://nmw.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://fvh.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yuf.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://etl.0kj1m.cn

Ruby: Dir.children("dir")
来源：http://gpi.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://qpg.52xcode.cn

[F09] 获取文件大小
来源：http://fnh.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://woa.yuxming.cn

PHP:  filesize("a.txt");
来源：http://pnx.xingfuxueyuan.xyz

JS:   fs.statSync("a.txt").size
来源：http://okd.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://dfp.vehdjk.com

Java: Files.size(Path.of("a.txt"))
来源：http://zeg.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nsd.iojbl.cn

Ruby: File.size("a.txt")
来源：http://kjs.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://npj.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://dpz.gotoacloud.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://guj.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sdn.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vmv.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://pby.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://upy.hammf.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://imr.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://trc.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uku.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://lrz.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kvu.sjlbkw.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ruh.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nyx.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lku.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gev.c1oappe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fwx.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hnh.wangdashe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://owi.daria6918.cn

[F12] CSV 读写
来源：http://khd.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cqx.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zvc.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yla.hfpthk.cn

TS:   // 同上
来源：http://ogl.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lug.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ngp.guowangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tzy.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vph.yfazqb.com

================================================================================
来源：http://lwe.redwolf501.top

G. 面向对象
来源：http://zgb.wangshuangyany.cn

================================================================================
来源：http://ccg.sjlbkw.cn

[G01] 定义类
来源：http://oxc.hywenlv.cn

Py:   class User: pass
来源：http://oyw.dashuyun.cn

PHP:  class User {}
来源：http://yap.yj20258888.top

JS:   class User {}
来源：http://tmr.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://fdk.xylfe.cn

Java: class User {}
来源：http://vuc.sufxvd.cn

Go:   type User struct { Name string }
来源：http://yae.dashuyun.cn

Ruby: class User; end
来源：http://uez.havefunace.top

C#:   class User {}
来源：http://qki.hammf.cn

[G02] 构造函数
来源：http://obi.tanke756.top

Py:   def __init__(self, name): self.name = name
来源：http://pjt.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://wbp.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://eyo.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://pyj.hfpthk.cn

Java: User(String name) { this.name = name; }
来源：http://suy.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mlu.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://sbd.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://zzz.wangshuangyany.cn

[G03] 实例属性
来源：http://uwr.hcnkem.com

Py:   self.name = "x"
来源：http://hiz.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://xac.zhongyouzk.top

JS:   this.name = "x";
来源：http://fbj.mhx1999.top

TS:   name: string = "x";
来源：http://hrd.epnwcf.com

Java: private String name;
来源：http://nwy.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iuq.haohaochexian.top

Ruby: @name = "x"
来源：http://iic.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://keo.guannengcc.top

[G04] 定义方法
来源：http://zfk.tian-w.cn

Py:   def greet(self): return self.name
来源：http://hli.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dnm.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://qjd.yueranfly.top

TS:   greet(): string { return this.name; }
来源：http://uzc.guannengcc.top

Java: String greet() { return name; }
来源：http://dow.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qhb.pycfn.com

Ruby: def greet; @name; end
来源：http://qhx.vehdjk.com

C#:   public string Greet() => Name;
来源：http://ayt.epnwcf.com

[G05] 继承
来源：http://mdn.nanxinkj.top

Py:   class Admin(User): pass
来源：http://cxh.mhx1999.top

PHP:  class Admin extends User {}
来源：http://wyo.yj20258888.top

JS:   class Admin extends User {}
来源：http://tmr.andypj.xyz

TS:   class Admin extends User {}
来源：http://tnf.chenjidiqi.icu

Java: class Admin extends User {}
来源：http://ide.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zut.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://jdk.birdmap.top

C#:   class Admin : User {}
来源：http://yag.cdnleiting.top

[G06] 重写方法
来源：http://ukh.shzxlz.cn

Py:   def greet(self): return "admin"
来源：http://mxa.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wex.pycfn.com

JS:   greet() { return "admin"; }
来源：http://mog.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://fgk.hywenlv.cn

Java: @Override String greet() { return "admin"; }
来源：http://tgr.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hcj.jinyuanbaomall.cn

Ruby: def greet; "admin"; end
来源：http://uyf.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://owm.jqgufenzy.top

[G07] 调用父类方法
来源：http://ymq.wangdashe.top

Py:   super().greet()
来源：http://ykc.nanxinkj.top

PHP:  parent::greet();
来源：http://sno.quarkkingdee.top

JS:   super.greet();
来源：http://diy.gotoacloud.top

TS:   super.greet();
来源：http://lly.pengpengdd.cyou

Java: super.greet();
来源：http://zad.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ijt.sufxvd.cn

Ruby: super
来源：http://roe.fengsongda.top

C#:   base.Greet();
来源：http://aza.shzxlz.cn

[G08] 静态方法与属性
来源：http://uab.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dev.jiagoushi.top

PHP:  public static function f() {}
来源：http://gqd.cqqwz.cn

JS:   static f() {}
来源：http://ecx.0kj1m.cn

TS:   static f(): void {}
来源：http://mhb.sysykeji.top

Java: static void f() {}
来源：http://fza.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://psp.fzhhl.top

Ruby: def self.f; end
来源：http://pkh.9152youxi.cn

C#:   public static void F() {}
来源：http://rju.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://czc.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://ack.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://doh.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ben.zhengqikj.top

TS:   interface Shape { area(): number; }
来源：http://qvb.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://ikz.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://xxw.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kav.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://pws.yvedp.cn

[G10] 访问控制
来源：http://goi.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://gnt.birdmap.top

PHP:  public / protected / private
来源：http://hzk.yonumen.top

JS:   #private 字段；其余公开
来源：http://kxw.tarul.cn

TS:   public / protected / private
来源：http://ydr.yonumen.top

Java: public / protected / private / 默认包级
来源：http://qqj.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oqt.hammf.cn

Ruby: public / protected / private
来源：http://kvx.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://uqx.daxiang520.top

[G11] getter / setter
来源：http://dgh.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://yly.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ftt.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://cxk.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://ifw.xylfe.cn

Java: public String getName() { return name; }
来源：http://frs.hcnkem.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ovp.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://hii.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://osz.smart0.xyz

[G12] 对象转字符串
来源：http://dsy.cucudq.cn

Py:   def __str__(self): return self.name
来源：http://npn.yj202588.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://plh.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://gmg.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://rmz.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://kgf.cashguo.top

Go:   func (u User) String() string { return u.Name }
来源：http://ymc.wangshuangyany.cn

Ruby: def to_s; @name; end
来源：http://wmp.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://rpl.zhixingplan.top

[G13] 判断对象类型
来源：http://txg.yonumen.top

Py:   isinstance(u, User)
来源：http://njv.sufxvd.cn

PHP:  $u instanceof User
来源：http://auc.mhx1999.top

JS:   u instanceof User
来源：http://oln.quarkkingdee.top

TS:   u instanceof User
来源：http://jie.mhx1999.top

Java: u instanceof User
来源：http://mxy.sjlbkw.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fdq.zhoulong.xyz

Ruby: u.is_a?(User)
来源：http://dhx.hnxiangtu.top

C#:   u is User
来源：http://oqv.tian-w.cn

[G14] 数据类 / record
来源：http://foa.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ece.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://gfj.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://qfr.pengpengdd.cyou

TS:   type User = { name: string; age: number };
来源：http://nds.iojbl.cn

Java: record User(String name, int age) {}
来源：http://evb.guowangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://gmx.iojbl.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qwb.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://xno.ydzc1.top

[G15] 枚举
来源：http://huy.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ahg.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vay.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qak.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lbe.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://ynn.fengsongda.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ebb.yj20258.top


<!-- 参考信息 -->