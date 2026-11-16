代发 wailian999

[E18] 模板占位符替换
来源：http://loq.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ngb.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hko.nwbrower.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mqf.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://chr.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mpd.meibo888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kjy.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://smv.xinyue.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bfc.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://iuw.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://msc.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://obg.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://tkt.jyoumei.cn

TS:   s.split(/\r?\n/)
来源：http://qgv.tian-w.cn

Java: s.lines().toList()
来源：http://tyi.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://ubf.svipenyu.cn

Ruby: s.lines
来源：http://czw.ppjwa.cn

C#:   s.Split('\n')
来源：http://uez.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://myq.jinqigfzy.top

Py:   if not s:
来源：http://kow.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://brt.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mwt.guannengcc.top

TS:   if (s === "") {}
来源：http://daq.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://nkc.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://mgf.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://muv.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tio.shzxlz.cn

[E21] 超长截断加省略号
来源：http://aqg.fengsongda.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yqd.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pvd.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dju.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mjm.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vgh.zhoulong.xyz

Go:   // 按 rune 判断长度后截断
来源：http://wis.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fbj.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rwk.meibo888.top

[E22] 字节长度与字符长度
来源：http://mqp.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rts.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jnr.hongshengwenyu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nnh.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wcl.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jxr.jlsjyb.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cqc.zhoulong.xyz

Ruby: s.bytesize;  s.length
来源：http://npo.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xue.zhiwuduotai.top

================================================================================
来源：http://tca.sufxvd.cn

F. 文件与目录
来源：http://fht.ehwqpu.com

================================================================================
来源：http://gjq.316326.xyz

[F01] 读取整个文件
来源：http://qmg.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pxo.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://son.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pnm.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dbf.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sle.tanke756.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lns.meibo888.top

Ruby: File.read("a.txt")
来源：http://gwx.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://uii.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://gro.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://clz.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qmf.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://izv.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gqe.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://urs.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lvz.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pnd.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yld.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://obt.ppjwa.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jfu.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kow.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nwx.yangfankeji.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lqg.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hiv.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ivg.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://qaa.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oeu.fehbvm.com

[F04] 追加写入文件
来源：http://ujg.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ezp.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vvu.9152youxi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tpy.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jaz.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gho.yvedp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xir.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zhr.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://whk.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://tgc.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yrc.shangyingyoupin.top

PHP:  file_exists("a.txt");
来源：http://ska.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://rdd.yj202588.top

TS:   fs.existsSync("a.txt")
来源：http://toa.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dso.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eze.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://bao.sufxvd.cn

C#:   File.Exists("a.txt")
来源：http://eic.ehwqpu.com

[F06] 删除文件
来源：http://oun.fzhhl.top

Py:   os.remove("a.txt")
来源：http://skf.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://rad.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nuq.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://gfs.zhiwuduotai.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ufr.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://cif.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://emr.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://pmv.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://jev.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gmd.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vfc.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xvj.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bft.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qak.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vne.bjfxy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yhe.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sdd.xinyue.icu

[F08] 遍历目录
来源：http://nar.haohaochexian.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jzh.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://isx.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://xav.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://vbq.aizwys.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fnt.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://oda.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://pfe.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://joi.tarul.cn

[F09] 获取文件大小
来源：http://uwm.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://wnp.chenlongwang.top

PHP:  filesize("a.txt");
来源：http://emy.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://zoq.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://ftc.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://hny.ydzc1.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pzs.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://tzo.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://jls.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://dgw.havefunace.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jji.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sic.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kmx.yj20258.top

TS:   path.extname("a.txt")
来源：http://xwt.guannengcc.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ohj.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vxq.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nma.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rea.quarkkingdee.top

[F11] 复制与移动文件
来源：http://fqr.vehdjk.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uby.chenlongwang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://twd.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gft.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fye.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bqj.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://otc.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://har.jqgufenzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vce.hfpthk.cn

[F12] CSV 读写
来源：http://jcg.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dgy.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zqd.zhijiandao.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://alb.cucudq.cn

TS:   // 同上
来源：http://ecl.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hmj.gaohongyu789.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kxa.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://imt.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ioe.zhongyouzk.top

================================================================================
来源：http://ilx.havefunace.top

G. 面向对象
来源：http://wvd.hfpthk.cn

================================================================================
来源：http://vij.jlsjyb.cn

[G01] 定义类
来源：http://qrv.daria6918.cn

Py:   class User: pass
来源：http://xfi.yvedp.cn

PHP:  class User {}
来源：http://jfv.yongpay.top

JS:   class User {}
来源：http://afh.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://xhg.hnqzz.top

Java: class User {}
来源：http://cxn.fanxiaobao.xyz

Go:   type User struct { Name string }
来源：http://trx.hysaishi.cn

Ruby: class User; end
来源：http://tdv.uphjek.com

C#:   class User {}
来源：http://wpr.tarul.cn

[G02] 构造函数
来源：http://cvr.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://dxm.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://uko.zhengqikj.top

JS:   constructor(name) { this.name = name; }
来源：http://dlc.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://lrh.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://okw.fktsv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qfe.shangyingyoupin.top

Ruby: def initialize(name); @name = name; end
来源：http://pis.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://bdd.sysykeji.top

[G03] 实例属性
来源：http://org.yonumen.top

Py:   self.name = "x"
来源：http://szb.cqqwz.cn

PHP:  public string $name = "x";
来源：http://geq.hesvh.cn

JS:   this.name = "x";
来源：http://lil.hesvh.cn

TS:   name: string = "x";
来源：http://kjx.hammf.cn

Java: private String name;
来源：http://zau.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://shj.andypj.xyz

Ruby: @name = "x"
来源：http://stj.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://ukl.gogol.net.cn

[G04] 定义方法
来源：http://wbf.nanxuanxn.top

Py:   def greet(self): return self.name
来源：http://fxa.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lxg.daria6918.cn

JS:   greet() { return this.name; }
来源：http://qdz.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://nqa.ivvv.top

Java: String greet() { return name; }
来源：http://ggf.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jel.tianlin.xyz

Ruby: def greet; @name; end
来源：http://vgs.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://blu.ywan-chungtsiang.top

[G05] 继承
来源：http://tmm.fanxiaobao.xyz

Py:   class Admin(User): pass
来源：http://cbj.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://iin.bbcook.cn

JS:   class Admin extends User {}
来源：http://mzd.tian-w.cn

TS:   class Admin extends User {}
来源：http://tgu.fengsongda.top

Java: class Admin extends User {}
来源：http://dpv.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qrh.vehdjk.com

Ruby: class Admin < User; end
来源：http://tug.bbcook.cn

C#:   class Admin : User {}
来源：http://jwn.quarkkingdee.top

[G06] 重写方法
来源：http://vsp.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://yfa.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jpt.daria6918.cn

JS:   greet() { return "admin"; }
来源：http://emf.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://ioo.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://zya.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ite.aibaodan.cn

Ruby: def greet; "admin"; end
来源：http://gvg.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://cqi.zhoulong.xyz

[G07] 调用父类方法
来源：http://pzo.jinqigufen.top

Py:   super().greet()
来源：http://zph.ydzc1.top

PHP:  parent::greet();
来源：http://tth.cdnleiting.top

JS:   super.greet();
来源：http://uyj.xinyue.icu

TS:   super.greet();
来源：http://uao.yvedp.cn

Java: super.greet();
来源：http://gzr.cdnleiting.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ryl.yongpay.top

Ruby: super
来源：http://chl.tianlin.xyz

C#:   base.Greet();
来源：http://qsj.c1oappe.top

[G08] 静态方法与属性
来源：http://dsm.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dfs.bjfxy.top

PHP:  public static function f() {}
来源：http://xxt.zycfv.cn

JS:   static f() {}
来源：http://boj.yj20258.top

TS:   static f(): void {}
来源：http://goh.smart0.xyz

Java: static void f() {}
来源：http://auf.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hab.52xcode.cn

Ruby: def self.f; end
来源：http://gfm.zhongyouzk.top

C#:   public static void F() {}
来源：http://lpb.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://wdn.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://lfo.vehdjk.com

PHP:  interface Shape { public function area(): float; }
来源：http://vxr.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jvj.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://egz.wangdashe.top

Java: interface Shape { double area(); }
来源：http://xuf.zhaomingkeji.xyz

Go:   type Shape interface { Area() float64 }
来源：http://fao.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tdh.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://rvh.yanxiufei.cn

[G10] 访问控制
来源：http://hob.jinyuanbaomall.cn

Py:   约定 _protected / __private（不强制）
来源：http://reg.xylfe.cn

PHP:  public / protected / private
来源：http://wvw.sweek.top

JS:   #private 字段；其余公开
来源：http://iyg.cqqwz.cn

TS:   public / protected / private
来源：http://wzi.zhijiandao.cn

Java: public / protected / private / 默认包级
来源：http://yei.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xjv.zycfv.cn

Ruby: public / protected / private
来源：http://fea.wangshuangyany.cn

C#:   public / protected / private / internal
来源：http://xmx.cucudq.cn

[G11] getter / setter
来源：http://wbt.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://zso.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://esn.sxryk.cn

JS:   get name() { return this._name; }
来源：http://sex.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://aim.havefunace.top

Java: public String getName() { return name; }
来源：http://yjh.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jyt.yfazqb.com

Ruby: attr_accessor :name
来源：http://bzv.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://iot.jinqigufen.top

[G12] 对象转字符串
来源：http://bgy.cashguo.top

Py:   def __str__(self): return self.name
来源：http://vnl.nanxuanxn.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bye.316326.xyz

JS:   toString() { return this.name; }
来源：http://mvx.hesvh.cn

TS:   toString(): string { return this.name; }
来源：http://pxx.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://xmx.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://paj.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://glx.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://htd.ybcxt.top

[G13] 判断对象类型
来源：http://cou.vehdjk.com

Py:   isinstance(u, User)
来源：http://xsa.ctjpmb.com

PHP:  $u instanceof User
来源：http://egd.ivvv.top

JS:   u instanceof User
来源：http://auc.iojbl.cn

TS:   u instanceof User
来源：http://tzs.sweek.top

Java: u instanceof User
来源：http://jlg.shanyushiyangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qnh.hnxiangtu.top

Ruby: u.is_a?(User)
来源：http://tts.9152youxi.cn

C#:   u is User
来源：http://joi.shzxlz.cn

[G14] 数据类 / record
来源：http://hvu.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mda.fengsongda.top

PHP:  // 用 readonly 属性模拟
来源：http://vic.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://vpx.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://zib.xuanzx.com

Java: record User(String name, int age) {}
来源：http://wyz.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://nzj.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xog.havefunace.top

C#:   record User(string Name, int Age);
来源：http://uzw.sufxvd.cn

[G15] 枚举
来源：http://kiy.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zcg.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ujj.pycfn.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vmt.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qim.vqdsnc.cn

Java: enum Color { RED, GREEN }
来源：http://fkn.sxryk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jpl.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://dbp.fzhhl.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tuz.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://rpn.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nna.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://ody.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://rir.ydzc1.top

TS:   Object.entries(obj)
来源：http://opy.hnxiangtu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://epb.zhiwuduotai.top


<!-- 参考信息 -->