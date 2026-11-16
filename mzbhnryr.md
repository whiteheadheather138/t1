代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vkl.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://viz.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xqs.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dpe.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ete.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sml.chenlongwang.top

Ruby: s.capitalize
来源：http://hzy.gaohongyu789.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sjr.yueranfly.top

[E18] 模板占位符替换
来源：http://hdy.yvedp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ahr.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cjc.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://bqp.xziqi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kda.svipenyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gjj.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fnt.hysaishi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://okh.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://coz.cheryme.top

[E19] 多行文本按行拆分
来源：http://phh.xinyue.icu

Py:   s.splitlines()
来源：http://ylz.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hzg.c1oappe.top

JS:   s.split(/\r?\n/)
来源：http://wzx.yonumen.top

TS:   s.split(/\r?\n/)
来源：http://ktj.iojbl.cn

Java: s.lines().toList()
来源：http://aid.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://hek.fanxiaobao.xyz

Ruby: s.lines
来源：http://pvh.jinyuanbaomall.cn

C#:   s.Split('\n')
来源：http://gzj.epnwcf.com

[E20] 判断字符串是否为空
来源：http://xof.ybcxt.top

Py:   if not s:
来源：http://ckg.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ybd.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ygc.jinqigufen.top

TS:   if (s === "") {}
来源：http://nlh.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://cle.yueranfly.top

Go:   if s == "" {}
来源：http://ljy.jiagoushi.top

Ruby: if s.empty?
来源：http://iuz.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uxl.dianchejie.cn

[E21] 超长截断加省略号
来源：http://wsk.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cth.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://emy.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rxf.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lcy.shanyushiyangtech.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oej.vqdsnc.cn

Go:   // 按 rune 判断长度后截断
来源：http://zrj.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bky.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sym.jqgufenzy.top

[E22] 字节长度与字符长度
来源：http://bde.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oha.xuanzx.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://izf.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mfl.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zlf.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hcs.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ltw.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://vqr.ehwqpu.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mwr.ehwqpu.com

================================================================================
来源：http://hmj.9152youxi.cn

F. 文件与目录
来源：http://ube.fehbvm.com

================================================================================
来源：http://bjj.vehdjk.com

[F01] 读取整个文件
来源：http://cab.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gjs.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://cmh.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eeo.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tlt.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xws.wangshuangyany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uwr.52xcode.cn

Ruby: File.read("a.txt")
来源：http://ifo.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://soo.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://nnc.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gjs.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dqj.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kal.cheryme.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://agm.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pxm.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fvl.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://djw.xuetiantiany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vrm.hysaishi.cn

[F03] 写入文件（覆盖）
来源：http://mqx.jiagoushi.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gul.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cey.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ped.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vhc.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rku.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qau.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://mst.jinghuilouyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vyb.yuanzhike.top

[F04] 追加写入文件
来源：http://kvb.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hmw.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yds.hesvh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://stg.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xqi.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://doe.zdqjudy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fpk.xingfuxueyuan.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ach.daria6918.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vhd.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://efn.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yir.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://agy.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://age.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://tde.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ygn.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ebl.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://zcu.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://eay.hesvh.cn

[F06] 删除文件
来源：http://uba.fehbvm.com

Py:   os.remove("a.txt")
来源：http://bpo.tanke756.top

PHP:  unlink("a.txt");
来源：http://tgr.wangdashe.top

JS:   fs.unlinkSync("a.txt")
来源：http://xhr.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://zit.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yfj.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://umc.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://qyc.316326.xyz

C#:   File.Delete("a.txt");
来源：http://atk.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://efu.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ylh.xylfe.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yhu.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bei.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gwm.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wse.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pqp.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://syb.pycfn.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ovx.yanxiufei.cn

[F08] 遍历目录
来源：http://jlu.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fie.snrcjt.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sgq.yueranfly.top

JS:   fs.readdirSync("dir")
来源：http://cxn.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://wez.gzhubu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jun.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xhs.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://vcf.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://dzx.epnwcf.com

[F09] 获取文件大小
来源：http://llv.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://exx.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://zsj.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://rgw.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://zro.pengpengdd.cyou

Java: Files.size(Path.of("a.txt"))
来源：http://bfv.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rvj.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://oub.fehbvm.com

C#:   new FileInfo("a.txt").Length
来源：http://yxm.tian-w.cn

[F10] 取文件扩展名 / 文件名
来源：http://amf.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rca.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qmh.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://otn.xziqi.cn

TS:   path.extname("a.txt")
来源：http://myz.tian-w.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qnl.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eju.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hmi.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eeo.bjfxy.top

[F11] 复制与移动文件
来源：http://aos.yvedp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mzl.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cit.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pti.chenzaomai.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kbi.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://irw.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gjs.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ihg.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nss.ydjk.org.cn

[F12] CSV 读写
来源：http://cxp.jyoumei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rfo.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lua.ppjwa.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wrp.zhongyouzk.top

TS:   // 同上
来源：http://aok.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xnn.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lfv.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mvm.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ztc.316326.xyz

================================================================================
来源：http://jev.kuanghao11.cn

G. 面向对象
来源：http://maq.jlsjyb.cn

================================================================================
来源：http://qwd.yueranfly.top

[G01] 定义类
来源：http://qkx.svipenyu.cn

Py:   class User: pass
来源：http://mob.ivvv.top

PHP:  class User {}
来源：http://bax.cdnleiting.top

JS:   class User {}
来源：http://pzg.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://dpx.yvedp.cn

Java: class User {}
来源：http://cdq.fktsv.cn

Go:   type User struct { Name string }
来源：http://uzg.zdqjudy.top

Ruby: class User; end
来源：http://rnk.vehdjk.com

C#:   class User {}
来源：http://bes.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://rcx.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://vkp.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://rxr.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ykf.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://xkd.zdbjq.cn

Java: User(String name) { this.name = name; }
来源：http://oyr.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fzf.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://ttv.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://ieg.chenzaomai.com

[G03] 实例属性
来源：http://kjr.yj20258888.top

Py:   self.name = "x"
来源：http://lve.fktsv.cn

PHP:  public string $name = "x";
来源：http://poe.hysaishi.cn

JS:   this.name = "x";
来源：http://ynu.uphjek.com

TS:   name: string = "x";
来源：http://ohy.jlsjyb.cn

Java: private String name;
来源：http://rha.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://clj.cheryme.top

Ruby: @name = "x"
来源：http://osw.guannengcc.top

C#:   public string Name { get; set; } = "x";
来源：http://ezh.nanxuanxn.top

[G04] 定义方法
来源：http://pyx.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://hkw.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bnd.haohaochexian.top

JS:   greet() { return this.name; }
来源：http://fpe.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://rsd.yueranfly.top

Java: String greet() { return name; }
来源：http://wrn.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://myf.uphjek.com

Ruby: def greet; @name; end
来源：http://jlw.ehwqpu.com

C#:   public string Greet() => Name;
来源：http://lem.zycfv.cn

[G05] 继承
来源：http://osf.jyoumei.cn

Py:   class Admin(User): pass
来源：http://alk.gzhubu.top

PHP:  class Admin extends User {}
来源：http://fha.yuanzhike.top

JS:   class Admin extends User {}
来源：http://utc.hnqzz.top

TS:   class Admin extends User {}
来源：http://rvh.xylfe.cn

Java: class Admin extends User {}
来源：http://nlk.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wzq.hywenlv.cn

Ruby: class Admin < User; end
来源：http://skp.havefunace.top

C#:   class Admin : User {}
来源：http://yre.yueranfly.top

[G06] 重写方法
来源：http://eip.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://oet.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bmy.yongpay.top

JS:   greet() { return "admin"; }
来源：http://vnz.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://dom.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://xcq.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cbv.tanke756.top

Ruby: def greet; "admin"; end
来源：http://yne.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://mgv.uphjek.com

[G07] 调用父类方法
来源：http://yrb.yonumen.top

Py:   super().greet()
来源：http://drm.cucudq.cn

PHP:  parent::greet();
来源：http://pku.tianlin.xyz

JS:   super.greet();
来源：http://ueo.redwolf501.top

TS:   super.greet();
来源：http://whw.guowangkeji.top

Java: super.greet();
来源：http://hhh.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://omi.yj202588.top

Ruby: super
来源：http://spy.jinqigufen.top

C#:   base.Greet();
来源：http://cpf.nanxuanxn.top

[G08] 静态方法与属性
来源：http://czo.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dwc.fehbvm.com

PHP:  public static function f() {}
来源：http://vyz.jinqigfzy.top

JS:   static f() {}
来源：http://eau.ehwqpu.com

TS:   static f(): void {}
来源：http://pcp.haohaochexian.top

Java: static void f() {}
来源：http://zrm.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dou.sweek.top

Ruby: def self.f; end
来源：http://uzk.bjfxy.top

C#:   public static void F() {}
来源：http://vsl.wangshuangyany.cn

[G09] 接口 / 抽象类
来源：http://nwk.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://con.zhijiandao.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jjy.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pjq.zdbjq.cn

TS:   interface Shape { area(): number; }
来源：http://fnj.fanxiaobao.xyz

Java: interface Shape { double area(); }
来源：http://mpq.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://iyx.cqqwz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eqb.aizwys.cn

C#:   interface IShape { double Area(); }
来源：http://ugi.vqdsnc.cn

[G10] 访问控制
来源：http://hwz.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://qin.xinyue.icu

PHP:  public / protected / private
来源：http://djv.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://tpx.cdnleiting.top

TS:   public / protected / private
来源：http://hpr.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://xns.fzhhl.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zuj.shanyushiyangtech.top

Ruby: public / protected / private
来源：http://ayb.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://oto.feifeiyinyue.top

[G11] getter / setter
来源：http://cbh.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://vky.yj20258888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dee.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://atr.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://uor.9152youxi.cn

Java: public String getName() { return name; }
来源：http://vyy.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gdl.jqgfzy.top

Ruby: attr_accessor :name
来源：http://cuk.xinyue.icu

C#:   public string Name { get; set; }
来源：http://mmk.c1oappe.top

[G12] 对象转字符串
来源：http://shs.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://cww.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zch.jyoumei.cn

JS:   toString() { return this.name; }
来源：http://kaq.tianlin.xyz

TS:   toString(): string { return this.name; }
来源：http://qbt.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://ffq.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://mqn.daxiang520.top

Ruby: def to_s; @name; end
来源：http://pbr.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://zvh.jianghu66.top

[G13] 判断对象类型
来源：http://cxu.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://tpo.iojbl.cn

PHP:  $u instanceof User
来源：http://dwv.epnwcf.com

JS:   u instanceof User
来源：http://wme.c1oappe.top

TS:   u instanceof User
来源：http://ezg.yj202588.top

Java: u instanceof User
来源：http://gsg.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://umj.hongshengwenyu.top

Ruby: u.is_a?(User)
来源：http://bfh.xuetiantiany.cn

C#:   u is User
来源：http://uve.cheryme.top

[G14] 数据类 / record
来源：http://asf.kuanghao11.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zzt.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://gmx.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://erk.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://gwh.ybcxt.top

Java: record User(String name, int age) {}
来源：http://vne.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://muh.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jag.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://iph.jinghuilouyu.cn

[G15] 枚举
来源：http://rpy.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xlg.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ufz.hesvh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kqi.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jml.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://ylp.yonumen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pje.zhixingplan.top


<!-- 参考信息 -->