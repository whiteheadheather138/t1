代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wqp.jinyuanbaomall.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qkz.hongshengwenyu.top

Ruby: s.capitalize
来源：http://lev.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tkx.chenzaomai.com

[E18] 模板占位符替换
来源：http://msl.jinqigfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pyq.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pob.pycfn.com

JS:   tpl.replaceAll("{name}", name)
来源：http://rpt.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cfz.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fne.yvedp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mij.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pby.9152youxi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tgv.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://crp.xinyue.icu

Py:   s.splitlines()
来源：http://fzq.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zxc.ydzc1.top

JS:   s.split(/\r?\n/)
来源：http://ydh.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://kry.uphjek.com

Java: s.lines().toList()
来源：http://zlu.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://oib.zhaomingkeji.xyz

Ruby: s.lines
来源：http://ybl.hcnkem.com

C#:   s.Split('\n')
来源：http://uhg.jiagoushi.top

[E20] 判断字符串是否为空
来源：http://tay.ydjk.org.cn

Py:   if not s:
来源：http://xxi.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yse.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://udd.0kj1m.cn

TS:   if (s === "") {}
来源：http://pye.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://xzi.yongpay.top

Go:   if s == "" {}
来源：http://zym.chenlongwang.top

Ruby: if s.empty?
来源：http://pnq.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bcf.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://tou.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fpl.sxryk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rsv.jiagoushi.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jqj.fengsongda.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kom.xingfuxueyuan.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hxf.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://mev.jinqigfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mzz.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ydr.hammf.cn

[E22] 字节长度与字符长度
来源：http://fky.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tkm.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://auy.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xbq.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rbt.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xva.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://knf.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://qcu.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hoe.meibo888.top

================================================================================
来源：http://che.zhixingplan.top

F. 文件与目录
来源：http://aac.yangfankeji.com

================================================================================
来源：http://scq.wangshuangyany.cn

[F01] 读取整个文件
来源：http://vob.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pmj.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://tsj.redwolf501.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fhb.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hzb.yj20258888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iuy.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dwh.ppjwa.cn

Ruby: File.read("a.txt")
来源：http://lto.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://xgp.daria6918.cn

[F02] 逐行读取文件
来源：http://vks.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dqi.chenlongwang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qdr.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qkg.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ggk.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tis.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://miz.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://muk.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ptu.cashguo.top

[F03] 写入文件（覆盖）
来源：http://ttg.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://soz.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qkm.zdqjudy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uhl.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tyb.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iqb.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xed.jlsjyb.cn

Ruby: File.write("a.txt", "hi")
来源：http://wkm.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hgl.zhijiandao.cn

[F04] 追加写入文件
来源：http://zjd.mhx1999.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gvk.yueranfly.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gvj.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iqo.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rpg.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cqa.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ahd.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jfg.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dvu.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://beh.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nrg.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://nxw.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://qdx.fzhhl.top

TS:   fs.existsSync("a.txt")
来源：http://lpj.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://bvj.wangdashe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://stl.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://ovm.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://tzs.quarkkingdee.top

[F06] 删除文件
来源：http://ner.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://zum.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://nhv.hnxiangtu.top

JS:   fs.unlinkSync("a.txt")
来源：http://ofv.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://oul.hywenlv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cdt.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://wtk.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://ljw.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://tpp.jianghu66.top

[F07] 创建目录（含多级）
来源：http://lgi.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gdj.bjfxy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ffy.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pcd.havefunace.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://giq.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://glu.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://prn.zycfv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rfl.hnqzz.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ysv.sjlbkw.cn

[F08] 遍历目录
来源：http://mmv.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://znc.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nez.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://lab.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://xix.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wgd.hnxiangtu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iig.tarul.cn

Ruby: Dir.children("dir")
来源：http://asl.hfpthk.cn

C#:   Directory.GetFiles("dir")
来源：http://yvx.jianghu66.top

[F09] 获取文件大小
来源：http://ljn.zdqjudy.top

Py:   os.path.getsize("a.txt")
来源：http://cqv.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://cag.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://noe.fengsongda.top

TS:   fs.statSync("a.txt").size
来源：http://bct.xingfuxueyuan.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://krz.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hpr.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://tfo.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://sxr.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://tps.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nzo.hongshengwenyu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qax.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cts.nwbrower.top

TS:   path.extname("a.txt")
来源：http://vdw.shuidangran.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bui.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ulu.xingfuxueyuan.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ygi.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gcq.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://ibj.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xxi.shangyingyoupin.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kop.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bdx.yanxiufei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mie.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aks.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://avk.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dsw.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hlb.quarkkingdee.top

[F12] CSV 读写
来源：http://mpv.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dcf.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://whp.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fjd.aizwys.cn

TS:   // 同上
来源：http://yjy.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nrp.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://poh.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yto.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://omu.dianchejie.cn

================================================================================
来源：http://dpq.yueranfly.top

G. 面向对象
来源：http://qaq.cashguo.top

================================================================================
来源：http://vdk.xuanzx.com

[G01] 定义类
来源：http://uhl.sweek.top

Py:   class User: pass
来源：http://mat.cheryme.top

PHP:  class User {}
来源：http://ztv.sweek.top

JS:   class User {}
来源：http://usk.jinghuilouyu.cn

TS:   class User { name: string = ""; }
来源：http://pla.xingfuxueyuan.xyz

Java: class User {}
来源：http://flo.wangdashe.top

Go:   type User struct { Name string }
来源：http://exz.cdnleiting.top

Ruby: class User; end
来源：http://qjw.quarkkingdee.top

C#:   class User {}
来源：http://ryv.aibaodan.cn

[G02] 构造函数
来源：http://dch.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://pzp.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://yuy.52xcode.cn

JS:   constructor(name) { this.name = name; }
来源：http://yil.chenzaomai.com

TS:   constructor(public name: string) {}
来源：http://llu.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://axp.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vuz.fengsongda.top

Ruby: def initialize(name); @name = name; end
来源：http://tzv.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://ihm.ywan-chungtsiang.top

[G03] 实例属性
来源：http://gdi.jqgfzy.top

Py:   self.name = "x"
来源：http://jzw.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://psd.zhongyouzk.top

JS:   this.name = "x";
来源：http://nes.zhiwuduotai.top

TS:   name: string = "x";
来源：http://tjm.jyoumei.cn

Java: private String name;
来源：http://zjf.yj202588.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fsr.cdnleiting.top

Ruby: @name = "x"
来源：http://xyq.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://azb.jyoumei.cn

[G04] 定义方法
来源：http://als.kuanghao11.cn

Py:   def greet(self): return self.name
来源：http://hzm.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dxq.yuanzhike.top

JS:   greet() { return this.name; }
来源：http://jgx.cqqwz.cn

TS:   greet(): string { return this.name; }
来源：http://uhg.aizwys.cn

Java: String greet() { return name; }
来源：http://rdn.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hnr.daxiang520.top

Ruby: def greet; @name; end
来源：http://emy.quarkkingdee.top

C#:   public string Greet() => Name;
来源：http://piq.zhoulong.xyz

[G05] 继承
来源：http://tfx.zhaomingkeji.xyz

Py:   class Admin(User): pass
来源：http://cqq.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://pia.yueranfly.top

JS:   class Admin extends User {}
来源：http://edc.smart0.xyz

TS:   class Admin extends User {}
来源：http://rxw.guannengcc.top

Java: class Admin extends User {}
来源：http://rwh.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fiz.zhaomingkeji.xyz

Ruby: class Admin < User; end
来源：http://bqu.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://plh.shzxlz.cn

[G06] 重写方法
来源：http://muh.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://ara.jqgfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pvp.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://tgv.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://qtr.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://twi.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://msv.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://qhs.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://xgw.zdqjudy.top

[G07] 调用父类方法
来源：http://sbw.hongshengwenyu.top

Py:   super().greet()
来源：http://krf.kuanghao11.cn

PHP:  parent::greet();
来源：http://vmw.dianchejie.cn

JS:   super.greet();
来源：http://fnu.yj202588.top

TS:   super.greet();
来源：http://boc.zhaomingkeji.xyz

Java: super.greet();
来源：http://haw.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://chm.hfpthk.cn

Ruby: super
来源：http://iba.yvedp.cn

C#:   base.Greet();
来源：http://mdv.daxiang520.top

[G08] 静态方法与属性
来源：http://gmd.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://goo.snrcjt.cn

PHP:  public static function f() {}
来源：http://fsr.bjfxy.top

JS:   static f() {}
来源：http://bib.jlsjyb.cn

TS:   static f(): void {}
来源：http://zxv.c1oappe.top

Java: static void f() {}
来源：http://cnz.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lbi.hywenlv.cn

Ruby: def self.f; end
来源：http://pfj.ehwqpu.com

C#:   public static void F() {}
来源：http://cfl.redwolf501.top

[G09] 接口 / 抽象类
来源：http://aep.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://xqm.ydzc1.top

PHP:  interface Shape { public function area(): float; }
来源：http://owm.hongshengwenyu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gje.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://hox.yvedp.cn

Java: interface Shape { double area(); }
来源：http://ejn.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://bcg.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://joa.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://fyn.wangdashe.top

[G10] 访问控制
来源：http://oyu.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://gyx.gotoacloud.top

PHP:  public / protected / private
来源：http://gdz.fktsv.cn

JS:   #private 字段；其余公开
来源：http://sah.vehdjk.com

TS:   public / protected / private
来源：http://azz.0kj1m.cn

Java: public / protected / private / 默认包级
来源：http://org.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://oav.hysaishi.cn

Ruby: public / protected / private
来源：http://hfz.gzhubu.top

C#:   public / protected / private / internal
来源：http://kva.shanyushiyangtech.top

[G11] getter / setter
来源：http://gri.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://kxl.0kj1m.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dce.yonumen.top

JS:   get name() { return this._name; }
来源：http://uhj.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://cef.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://row.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gpr.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://jew.bbcook.cn

C#:   public string Name { get; set; }
来源：http://umu.cheryme.top

[G12] 对象转字符串
来源：http://ktj.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://jtc.nanxuanxn.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://scu.sweek.top

JS:   toString() { return this.name; }
来源：http://yxt.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://vpi.fengsongda.top

Java: @Override public String toString() { return name; }
来源：http://crk.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://uhi.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://yhe.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://qis.jqgufenzy.top

[G13] 判断对象类型
来源：http://sxz.hesvh.cn

Py:   isinstance(u, User)
来源：http://qhi.tianlin.xyz

PHP:  $u instanceof User
来源：http://yps.yanxiufei.cn

JS:   u instanceof User
来源：http://xmk.epnwcf.com

TS:   u instanceof User
来源：http://opd.sysykeji.top

Java: u instanceof User
来源：http://neu.cheryme.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zgn.316326.xyz

Ruby: u.is_a?(User)
来源：http://ilg.hcnkem.com

C#:   u is User
来源：http://gig.cucudq.cn

[G14] 数据类 / record
来源：http://hav.yangfankeji.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mqk.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://cxw.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://yrs.ydjk.org.cn

TS:   type User = { name: string; age: number };
来源：http://kcg.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://lvh.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://ooz.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ruz.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://fnk.cashguo.top

[G15] 枚举
来源：http://knw.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://unm.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xlf.yueranfly.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gud.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yyp.jianghu66.top

Java: enum Color { RED, GREEN }
来源：http://slx.fehbvm.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hrc.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://xdz.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://twz.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://xfs.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zkj.cucudq.cn


<!-- 参考信息 -->