代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eft.sysykeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ela.kuanghao11.cn

Ruby: s.capitalize
来源：http://jko.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://muz.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://lhq.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qsv.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fus.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ggg.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://fxc.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dtl.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lvy.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://abf.sufxvd.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jee.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://tlw.xuanzx.com

Py:   s.splitlines()
来源：http://jkz.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lix.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://lmz.yongpay.top

TS:   s.split(/\r?\n/)
来源：http://xri.hysaishi.cn

Java: s.lines().toList()
来源：http://eav.shanyushiyangtech.top

Go:   strings.Split(s, "\n")
来源：http://rid.yuxming.cn

Ruby: s.lines
来源：http://zph.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://bjz.xuanzx.com

[E20] 判断字符串是否为空
来源：http://fwe.xinyue.icu

Py:   if not s:
来源：http://eju.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lze.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xws.gzhubu.top

TS:   if (s === "") {}
来源：http://kzm.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://bdt.cucudq.cn

Go:   if s == "" {}
来源：http://otm.dashuyun.cn

Ruby: if s.empty?
来源：http://tli.jianghu66.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nle.shanyushiyangtech.top

[E21] 超长截断加省略号
来源：http://vjo.aibaodan.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ykv.zycfv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qbk.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fic.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uvi.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mat.gaohongyu789.top

Go:   // 按 rune 判断长度后截断
来源：http://eju.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://knm.dianchejie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ugj.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://xpy.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fzp.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kfr.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kyu.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gra.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ofp.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xlg.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://ohi.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zju.zhiwuduotai.top

================================================================================
来源：http://msr.bjfxy.top

F. 文件与目录
来源：http://xdx.xingfuxueyuan.xyz

================================================================================
来源：http://ila.hnxiangtu.top

[F01] 读取整个文件
来源：http://eua.aibaodan.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uqj.jqgfzy.top

PHP:  file_get_contents("a.txt");
来源：http://imv.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://azc.fehbvm.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oza.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ovh.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mgj.gzhubu.top

Ruby: File.read("a.txt")
来源：http://zbo.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://rbo.redwolf501.top

[F02] 逐行读取文件
来源：http://vjk.mhx1999.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ehw.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bmt.tian-w.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bhd.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://efq.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uek.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://apu.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oms.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://czh.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://ymn.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://all.jianghu66.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dxr.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yjm.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fgp.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://smk.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kte.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://yin.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xvw.yvedp.cn

[F04] 追加写入文件
来源：http://sob.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ndw.hfpthk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dax.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pbp.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kim.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hui.shanyushiyangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://faa.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nkm.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tgy.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://gjw.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jwo.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://ank.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://fzw.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://nnq.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vwr.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vqx.ctjpmb.com

Ruby: File.exist?("a.txt")
来源：http://rri.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://lle.gzhubu.top

[F06] 删除文件
来源：http://wcj.jinyuanbaomall.cn

Py:   os.remove("a.txt")
来源：http://dwm.sxryk.cn

PHP:  unlink("a.txt");
来源：http://lcy.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://ndw.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://emr.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uos.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://fcz.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://bkx.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://kzj.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://cdu.andypj.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uji.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fma.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dgx.yvedp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eiy.kuanghao11.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gxr.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ifs.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jzm.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://isb.ctjpmb.com

[F08] 遍历目录
来源：http://ftv.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lgj.jinghuilouyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sxp.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://aua.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://sop.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hsz.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pnn.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://zge.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://znc.wangshuangyany.cn

[F09] 获取文件大小
来源：http://ghf.shanyushiyangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://onp.hywenlv.cn

PHP:  filesize("a.txt");
来源：http://rlx.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://gdp.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://fvu.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://pyi.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://giz.shuidangran.top

Ruby: File.size("a.txt")
来源：http://azl.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://fof.yvedp.cn

[F10] 取文件扩展名 / 文件名
来源：http://zgm.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://awn.svipenyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://alt.zhengqikj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zcl.meibo888.top

TS:   path.extname("a.txt")
来源：http://tlu.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jdh.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://krb.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kua.zdbjq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bgq.bjfxy.top

[F11] 复制与移动文件
来源：http://xdr.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kvb.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nir.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hgs.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bri.hesvh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ocx.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ukq.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xei.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dsg.gogol.net.cn

[F12] CSV 读写
来源：http://crn.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hzu.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cpe.chenzaomai.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eps.shangyingyoupin.top

TS:   // 同上
来源：http://ycj.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://suw.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eza.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xwy.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ylp.cdnleiting.top

================================================================================
来源：http://qnl.hnxiangtu.top

G. 面向对象
来源：http://lmf.nanxinkj.top

================================================================================
来源：http://ppd.cqqwz.cn

[G01] 定义类
来源：http://tdv.fehbvm.com

Py:   class User: pass
来源：http://npz.hcnkem.com

PHP:  class User {}
来源：http://srh.wangdashe.top

JS:   class User {}
来源：http://blc.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://xub.fehbvm.com

Java: class User {}
来源：http://tbf.hfpthk.cn

Go:   type User struct { Name string }
来源：http://vgb.jinyuanbaomall.cn

Ruby: class User; end
来源：http://til.zdbjq.cn

C#:   class User {}
来源：http://ibl.yuxming.cn

[G02] 构造函数
来源：http://dqx.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://zww.ppjwa.cn

PHP:  public function __construct(public string $name) {}
来源：http://ebm.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://ssu.hysaishi.cn

TS:   constructor(public name: string) {}
来源：http://fzw.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://qai.sxryk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ixn.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://hmy.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://ceo.hfpthk.cn

[G03] 实例属性
来源：http://qot.xuetiantiany.cn

Py:   self.name = "x"
来源：http://wcc.guowangkeji.top

PHP:  public string $name = "x";
来源：http://amu.yj20258888.top

JS:   this.name = "x";
来源：http://hpp.wangshuangyany.cn

TS:   name: string = "x";
来源：http://dtg.hysaishi.cn

Java: private String name;
来源：http://cbq.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lwh.nwbrower.top

Ruby: @name = "x"
来源：http://gkk.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://tnf.ctjpmb.com

[G04] 定义方法
来源：http://rdz.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://fzz.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sbm.aibaodan.cn

JS:   greet() { return this.name; }
来源：http://cqb.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://vba.ydjk.org.cn

Java: String greet() { return name; }
来源：http://pop.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fao.yuanzhike.top

Ruby: def greet; @name; end
来源：http://iiy.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://odq.xylfe.cn

[G05] 继承
来源：http://vcx.shangyingyoupin.top

Py:   class Admin(User): pass
来源：http://qhl.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://fub.vehdjk.com

JS:   class Admin extends User {}
来源：http://ieh.ivvv.top

TS:   class Admin extends User {}
来源：http://oav.jinqigufen.top

Java: class Admin extends User {}
来源：http://gub.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cae.yuanzhike.top

Ruby: class Admin < User; end
来源：http://wej.zhoulong.xyz

C#:   class Admin : User {}
来源：http://sbt.ybcxt.top

[G06] 重写方法
来源：http://ltk.chenzaomai.com

Py:   def greet(self): return "admin"
来源：http://bpl.dianchejie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sqi.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://prv.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://lrm.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://aod.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ghe.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://zvo.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://vnb.pycfn.com

[G07] 调用父类方法
来源：http://knn.wangshuangyany.cn

Py:   super().greet()
来源：http://ogd.shangyingyoupin.top

PHP:  parent::greet();
来源：http://njx.c1oappe.top

JS:   super.greet();
来源：http://yth.shzxlz.cn

TS:   super.greet();
来源：http://nqs.dianchejie.cn

Java: super.greet();
来源：http://cdz.jyoumei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mkb.guowangkeji.top

Ruby: super
来源：http://qov.uphjek.com

C#:   base.Greet();
来源：http://cgg.9152youxi.cn

[G08] 静态方法与属性
来源：http://qoc.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fyc.ivvv.top

PHP:  public static function f() {}
来源：http://cqc.snrcjt.cn

JS:   static f() {}
来源：http://zwz.yj20258.top

TS:   static f(): void {}
来源：http://imh.quarkkingdee.top

Java: static void f() {}
来源：http://dby.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rrg.cucudq.cn

Ruby: def self.f; end
来源：http://ynm.hnqzz.top

C#:   public static void F() {}
来源：http://hab.gotoacloud.top

[G09] 接口 / 抽象类
来源：http://ghq.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://xdh.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bjc.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mtn.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://bnn.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://qmm.hammf.cn

Go:   type Shape interface { Area() float64 }
来源：http://ogl.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://szm.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://cbz.yuxming.cn

[G10] 访问控制
来源：http://til.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://pva.nwbrower.top

PHP:  public / protected / private
来源：http://icb.fzhhl.top

JS:   #private 字段；其余公开
来源：http://ucl.tianlin.xyz

TS:   public / protected / private
来源：http://sci.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://hxn.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mxd.yangfankeji.com

Ruby: public / protected / private
来源：http://qhp.fktsv.cn

C#:   public / protected / private / internal
来源：http://yzb.0kj1m.cn

[G11] getter / setter
来源：http://xnl.ybcxt.top

Py:   @property 与 @x.setter
来源：http://ieo.gogol.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fik.bbcook.cn

JS:   get name() { return this._name; }
来源：http://nus.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://zpx.zdbjq.cn

Java: public String getName() { return name; }
来源：http://wdp.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dqc.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://vti.sxryk.cn

C#:   public string Name { get; set; }
来源：http://twy.shzxlz.cn

[G12] 对象转字符串
来源：http://nbv.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://lka.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tdj.shuidangran.top

JS:   toString() { return this.name; }
来源：http://amj.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://hto.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://kdh.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://esh.yueranfly.top

Ruby: def to_s; @name; end
来源：http://wob.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://mty.tian-w.cn

[G13] 判断对象类型
来源：http://hmz.sxryk.cn

Py:   isinstance(u, User)
来源：http://zqi.cdnleiting.top

PHP:  $u instanceof User
来源：http://qux.xuetiantiany.cn

JS:   u instanceof User
来源：http://nvb.316326.xyz

TS:   u instanceof User
来源：http://ymo.guowangkeji.top

Java: u instanceof User
来源：http://ptg.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uyo.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://jar.sxryk.cn

C#:   u is User
来源：http://hrm.gzhubu.top

[G14] 数据类 / record
来源：http://psc.gaohongyu789.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xeh.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://ozc.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://eqb.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://csz.zycfv.cn

Java: record User(String name, int age) {}
来源：http://qog.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://yrt.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rcb.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://ziv.ydjk.org.cn

[G15] 枚举
来源：http://cdy.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ayj.yvedp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rag.daria6918.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ihu.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aqy.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://sbk.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://phv.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://mtk.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://anz.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://ino.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ers.hammf.cn


<!-- 参考信息 -->