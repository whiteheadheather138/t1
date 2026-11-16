代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bbq.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://opt.vqdsnc.cn

Ruby: s.capitalize
来源：http://zzl.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rtw.redwolf501.top

[E18] 模板占位符替换
来源：http://lrh.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rid.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gxz.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gjx.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lmu.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tnl.gogol.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uxe.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://muu.aibaodan.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zuk.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://zeg.dianchejie.cn

Py:   s.splitlines()
来源：http://jcf.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jtd.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://lea.jiagoushi.top

TS:   s.split(/\r?\n/)
来源：http://syd.daria6918.cn

Java: s.lines().toList()
来源：http://xxt.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://svy.ivvv.top

Ruby: s.lines
来源：http://mog.52xcode.cn

C#:   s.Split('\n')
来源：http://cre.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://sjc.xuetiantiany.cn

Py:   if not s:
来源：http://psw.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://prk.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gix.yangfankeji.com

TS:   if (s === "") {}
来源：http://myg.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://ass.hongshengwenyu.top

Go:   if s == "" {}
来源：http://hgr.yongpay.top

Ruby: if s.empty?
来源：http://lmz.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ydj.tanke756.top

[E21] 超长截断加省略号
来源：http://pez.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://idy.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ixh.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yvl.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ygo.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ste.svipenyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://wuc.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ldm.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kkl.sxryk.cn

[E22] 字节长度与字符长度
来源：http://pso.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ofw.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://unj.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nlr.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uig.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://atl.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nvk.daxiang520.top

Ruby: s.bytesize;  s.length
来源：http://den.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qle.yongpay.top

================================================================================
来源：http://gzm.0kj1m.cn

F. 文件与目录
来源：http://edb.shanyushiyangtech.top

================================================================================
来源：http://zco.cdnleiting.top

[F01] 读取整个文件
来源：http://wzz.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://guc.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://oda.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cjt.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fti.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qgh.zycfv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ezb.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://yzr.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://zah.shzxlz.cn

[F02] 逐行读取文件
来源：http://csx.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tmc.yfazqb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://amv.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gss.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aiy.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gvd.316326.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yel.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://azn.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rxr.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://tif.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vkl.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oej.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rja.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mbj.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dna.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mmp.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://scr.xinyue.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gno.yongpay.top

[F04] 追加写入文件
来源：http://wvs.hnqzz.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kiy.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rxc.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zzq.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jum.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yid.zhongyouzk.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vkj.xingfuxueyuan.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hih.aibaodan.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rif.aizwys.cn

[F05] 判断文件或目录是否存在
来源：http://lqi.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aol.zhixingplan.top

PHP:  file_exists("a.txt");
来源：http://euj.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://tpq.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://mpd.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://mgw.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tgk.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://jwj.birdmap.top

C#:   File.Exists("a.txt")
来源：http://ozm.gzhubu.top

[F06] 删除文件
来源：http://tbc.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://mrb.nanxinkj.top

PHP:  unlink("a.txt");
来源：http://mok.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://fvn.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://xyd.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ghd.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://dbb.jianghu66.top

Ruby: File.delete("a.txt")
来源：http://paf.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://pyg.xuanzx.com

[F07] 创建目录（含多级）
来源：http://tuu.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nqi.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://khq.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://agl.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mgo.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fck.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qrr.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dud.jlsjyb.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iuj.aibaodan.cn

[F08] 遍历目录
来源：http://cku.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zrb.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ntx.gzhubu.top

JS:   fs.readdirSync("dir")
来源：http://wmm.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://euk.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hnw.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://chg.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://luz.ehwqpu.com

C#:   Directory.GetFiles("dir")
来源：http://mrb.9152youxi.cn

[F09] 获取文件大小
来源：http://ymu.uphjek.com

Py:   os.path.getsize("a.txt")
来源：http://uqe.316326.xyz

PHP:  filesize("a.txt");
来源：http://cvv.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://wjr.tanke756.top

TS:   fs.statSync("a.txt").size
来源：http://ydv.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://rqh.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qxm.daxiang520.top

Ruby: File.size("a.txt")
来源：http://yev.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://sri.sxryk.cn

[F10] 取文件扩展名 / 文件名
来源：http://dyp.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kmt.fanxiaobao.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qii.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://azp.sysykeji.top

TS:   path.extname("a.txt")
来源：http://zkb.guannengcc.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hja.0kj1m.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://imj.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ksg.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dba.hnqzz.top

[F11] 复制与移动文件
来源：http://nqk.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dam.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sov.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zcr.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vaw.ywan-chungtsiang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xkf.jianghu66.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kco.xingfuxueyuan.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bbv.chenlongwang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iqp.hywenlv.cn

[F12] CSV 读写
来源：http://xfo.cqqwz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hem.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jmj.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hpi.shuidangran.top

TS:   // 同上
来源：http://tfu.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dfm.fengsongda.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wmp.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lik.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lbo.gzhubu.top

================================================================================
来源：http://iys.yvedp.cn

G. 面向对象
来源：http://hin.gotoacloud.top

================================================================================
来源：http://uoy.jqgufenzy.top

[G01] 定义类
来源：http://fvk.zhiwuduotai.top

Py:   class User: pass
来源：http://wcx.yonumen.top

PHP:  class User {}
来源：http://lum.jqgufenzy.top

JS:   class User {}
来源：http://amb.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://aoz.zdqjudy.top

Java: class User {}
来源：http://tno.xylfe.cn

Go:   type User struct { Name string }
来源：http://pvj.zhixingplan.top

Ruby: class User; end
来源：http://cpk.hywenlv.cn

C#:   class User {}
来源：http://wfr.sysykeji.top

[G02] 构造函数
来源：http://rat.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://auy.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://gdn.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://jja.ctjpmb.com

TS:   constructor(public name: string) {}
来源：http://xms.shanyushiyangtech.top

Java: User(String name) { this.name = name; }
来源：http://bhi.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jfk.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://cxi.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://avg.sjlbkw.cn

[G03] 实例属性
来源：http://bwb.kuanghao11.cn

Py:   self.name = "x"
来源：http://hdc.dianchejie.cn

PHP:  public string $name = "x";
来源：http://txp.gogol.net.cn

JS:   this.name = "x";
来源：http://eqh.chenjidiqi.icu

TS:   name: string = "x";
来源：http://rvp.hywenlv.cn

Java: private String name;
来源：http://pcg.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kqj.gogol.net.cn

Ruby: @name = "x"
来源：http://hur.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://qwd.hcnkem.com

[G04] 定义方法
来源：http://frz.ehwqpu.com

Py:   def greet(self): return self.name
来源：http://bpj.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uxx.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://yox.hammf.cn

TS:   greet(): string { return this.name; }
来源：http://nno.yueranfly.top

Java: String greet() { return name; }
来源：http://rqr.uphjek.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://lnb.hywenlv.cn

Ruby: def greet; @name; end
来源：http://pln.redwolf501.top

C#:   public string Greet() => Name;
来源：http://upk.zhixingplan.top

[G05] 继承
来源：http://cbv.birdmap.top

Py:   class Admin(User): pass
来源：http://bzu.quarkkingdee.top

PHP:  class Admin extends User {}
来源：http://zqb.hcnkem.com

JS:   class Admin extends User {}
来源：http://edy.dianchejie.cn

TS:   class Admin extends User {}
来源：http://asc.cucudq.cn

Java: class Admin extends User {}
来源：http://voa.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xud.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://wkp.ybcxt.top

C#:   class Admin : User {}
来源：http://wgp.wangshuangyany.cn

[G06] 重写方法
来源：http://pre.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://gwp.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vlo.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://vds.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://diy.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://nnw.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://svy.zdqjudy.top

Ruby: def greet; "admin"; end
来源：http://kiv.nwbrower.top

C#:   public override string Greet() => "admin";
来源：http://hqb.zhongyouzk.top

[G07] 调用父类方法
来源：http://syy.cdnleiting.top

Py:   super().greet()
来源：http://nvx.yuanzhike.top

PHP:  parent::greet();
来源：http://fyi.52xcode.cn

JS:   super.greet();
来源：http://gun.tian-w.cn

TS:   super.greet();
来源：http://ijl.zycfv.cn

Java: super.greet();
来源：http://mgn.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vzj.hcnkem.com

Ruby: super
来源：http://bzp.hongshengwenyu.top

C#:   base.Greet();
来源：http://bdj.jianghu66.top

[G08] 静态方法与属性
来源：http://vde.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oeu.shanyushiyangkeji.top

PHP:  public static function f() {}
来源：http://hka.xziqi.cn

JS:   static f() {}
来源：http://tjf.epnwcf.com

TS:   static f(): void {}
来源：http://kzi.tarul.cn

Java: static void f() {}
来源：http://bin.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://tdf.hongshengwenyu.top

Ruby: def self.f; end
来源：http://nkn.wangshuangyany.cn

C#:   public static void F() {}
来源：http://gns.fzhhl.top

[G09] 接口 / 抽象类
来源：http://zbm.bbcook.cn

Py:   from abc import ABC, abstractmethod
来源：http://izq.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://lhk.xylfe.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://naa.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://pmf.jianghu66.top

Java: interface Shape { double area(); }
来源：http://mkf.gotoacloud.top

Go:   type Shape interface { Area() float64 }
来源：http://iyt.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ghe.yj20258888.top

C#:   interface IShape { double Area(); }
来源：http://pkz.fehbvm.com

[G10] 访问控制
来源：http://sox.tanke756.top

Py:   约定 _protected / __private（不强制）
来源：http://jcg.c1oappe.top

PHP:  public / protected / private
来源：http://umi.yj20258888.top

JS:   #private 字段；其余公开
来源：http://lno.gotoacloud.top

TS:   public / protected / private
来源：http://cqt.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://ygv.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://sej.sjlbkw.cn

Ruby: public / protected / private
来源：http://bym.xuanzx.com

C#:   public / protected / private / internal
来源：http://rbf.tanke756.top

[G11] getter / setter
来源：http://qpq.chenlongwang.top

Py:   @property 与 @x.setter
来源：http://gjl.sxryk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dfs.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://ykb.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://sbr.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://jsw.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vvf.zycfv.cn

Ruby: attr_accessor :name
来源：http://vop.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://jjf.gogol.net.cn

[G12] 对象转字符串
来源：http://ndj.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://yqx.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kjm.yj20258.top

JS:   toString() { return this.name; }
来源：http://gxy.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://bhp.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://edl.jinqigufen.top

Go:   func (u User) String() string { return u.Name }
来源：http://wfm.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://dvb.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://fap.sxryk.cn

[G13] 判断对象类型
来源：http://mqe.xuanzx.com

Py:   isinstance(u, User)
来源：http://pjn.gotoacloud.top

PHP:  $u instanceof User
来源：http://imb.fehbvm.com

JS:   u instanceof User
来源：http://ilx.zhiwuduotai.top

TS:   u instanceof User
来源：http://ayz.nanxinkj.top

Java: u instanceof User
来源：http://zyf.jyoumei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zkz.zycfv.cn

Ruby: u.is_a?(User)
来源：http://ypv.jianghu66.top

C#:   u is User
来源：http://gmu.cqqwz.cn

[G14] 数据类 / record
来源：http://owi.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cop.yueranfly.top

PHP:  // 用 readonly 属性模拟
来源：http://yqy.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ewx.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://qlx.yonumen.top

Java: record User(String name, int age) {}
来源：http://vmc.zhaomingkeji.xyz

Go:   type User struct { Name string; Age int }
来源：http://tte.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://icu.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://kss.epnwcf.com

[G15] 枚举
来源：http://htn.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wpy.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rdv.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hwd.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cxv.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://lll.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hyc.nanxuanxn.top

Ruby: Color = %i[red green].freeze
来源：http://gwo.yanxiufei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oru.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://ddy.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pyl.zhixingplan.top


<!-- 参考信息 -->