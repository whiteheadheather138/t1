代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bzv.epnwcf.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gzl.yj20258.top

Ruby: s.capitalize
来源：http://hip.yj20258.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xvy.sxryk.cn

[E18] 模板占位符替换
来源：http://mwq.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cid.zdbjq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://afu.pengpengdd.cyou

JS:   tpl.replaceAll("{name}", name)
来源：http://taj.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ztw.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fxc.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tyh.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mmm.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qmb.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://tpj.kuanghao11.cn

Py:   s.splitlines()
来源：http://equ.zdbjq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oki.zhiwuduotai.top

JS:   s.split(/\r?\n/)
来源：http://sci.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://cci.ydjk.org.cn

Java: s.lines().toList()
来源：http://tyy.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://lew.hnqzz.top

Ruby: s.lines
来源：http://yvk.hysaishi.cn

C#:   s.Split('\n')
来源：http://wnq.yueranfly.top

[E20] 判断字符串是否为空
来源：http://lmz.yj20258.top

Py:   if not s:
来源：http://smm.cheryme.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ahd.andypj.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jue.ybcxt.top

TS:   if (s === "") {}
来源：http://lsc.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://vgy.yuanzhike.top

Go:   if s == "" {}
来源：http://vey.9152youxi.cn

Ruby: if s.empty?
来源：http://zqz.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qzi.hongshengwenyu.top

[E21] 超长截断加省略号
来源：http://pug.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ekz.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xdc.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oeg.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gtm.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tpt.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://twx.xziqi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ifl.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iwc.hcnkem.com

[E22] 字节长度与字符长度
来源：http://esv.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uzg.jqgufenzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nvs.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://euz.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rlj.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mhw.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://phx.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://zpb.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vqh.snrcjt.cn

================================================================================
来源：http://voe.gzhubu.top

F. 文件与目录
来源：http://krp.andypj.xyz

================================================================================
来源：http://mjo.epnwcf.com

[F01] 读取整个文件
来源：http://qau.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://shd.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://cck.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kso.jinyuanbaomall.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sql.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ain.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ryt.yj202588.top

Ruby: File.read("a.txt")
来源：http://sdy.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://sxn.hfpthk.cn

[F02] 逐行读取文件
来源：http://oaj.cheryme.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bws.fehbvm.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bou.birdmap.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pbf.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ltj.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oen.yongpay.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://azl.zhongyouzk.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://emn.jqgufenzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qye.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://bem.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aog.jianghu66.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bms.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ksn.quarkkingdee.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yeb.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://opn.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fsy.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://ybz.haohaochexian.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eiu.ydzc1.top

[F04] 追加写入文件
来源：http://tzz.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eto.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cex.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jcn.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qcx.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mfk.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hhm.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yvm.zhengqikj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bzx.dashuyun.cn

[F05] 判断文件或目录是否存在
来源：http://bqt.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tew.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://hon.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://ppy.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://xpr.guannengcc.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vwo.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tzs.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://ity.yj20258888.top

C#:   File.Exists("a.txt")
来源：http://hpd.chenlongwang.top

[F06] 删除文件
来源：http://lbv.jinyuanbaomall.cn

Py:   os.remove("a.txt")
来源：http://utx.nwbrower.top

PHP:  unlink("a.txt");
来源：http://agp.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://bnz.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dso.yueranfly.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cek.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://uoi.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://opw.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://psr.pengpengdd.cyou

[F07] 创建目录（含多级）
来源：http://bnv.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ayc.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yjw.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gou.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tze.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lmq.jyoumei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://usn.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yzb.shuidangran.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mlg.zdqjudy.top

[F08] 遍历目录
来源：http://nyi.fktsv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yat.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tlq.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://ovo.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://bdt.c1oappe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ivp.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://djp.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://wqb.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://ibj.vehdjk.com

[F09] 获取文件大小
来源：http://cla.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://tsz.ctjpmb.com

PHP:  filesize("a.txt");
来源：http://xqj.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://tex.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://ihv.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mtt.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xwg.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://zqv.hcnkem.com

C#:   new FileInfo("a.txt").Length
来源：http://qym.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://ect.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hco.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kfr.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yqf.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://txb.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://whq.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mey.redwolf501.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dmo.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://geh.hongshengwenyu.top

[F11] 复制与移动文件
来源：http://yxc.yueranfly.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qtw.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bgn.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ncl.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fxz.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nms.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oeg.chenjidiqi.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xdl.smart0.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ham.hammf.cn

[F12] CSV 读写
来源：http://lwy.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mud.daria6918.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://njw.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hma.nanxuanxn.top

TS:   // 同上
来源：http://poz.hcnkem.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hmt.ydzc1.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ckp.shangyingyoupin.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://txu.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://zii.zycfv.cn

================================================================================
来源：http://chl.aizwys.cn

G. 面向对象
来源：http://zld.shuidangran.top

================================================================================
来源：http://aro.316326.xyz

[G01] 定义类
来源：http://jml.aibaodan.cn

Py:   class User: pass
来源：http://xru.daxiang520.top

PHP:  class User {}
来源：http://ppe.cdnleiting.top

JS:   class User {}
来源：http://mkm.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://lvi.chenlongwang.top

Java: class User {}
来源：http://nlc.wangdashe.top

Go:   type User struct { Name string }
来源：http://rrf.gogol.net.cn

Ruby: class User; end
来源：http://lsv.fzhhl.top

C#:   class User {}
来源：http://fyl.hysaishi.cn

[G02] 构造函数
来源：http://ryl.jqgufenzy.top

Py:   def __init__(self, name): self.name = name
来源：http://fpu.pengpengdd.cyou

PHP:  public function __construct(public string $name) {}
来源：http://jlb.gogol.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://gax.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://dew.fktsv.cn

Java: User(String name) { this.name = name; }
来源：http://chw.hesvh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://urm.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://nlo.redwolf501.top

C#:   public User(string name) { Name = name; }
来源：http://rwu.tian-w.cn

[G03] 实例属性
来源：http://szv.svipenyu.cn

Py:   self.name = "x"
来源：http://rmt.yvedp.cn

PHP:  public string $name = "x";
来源：http://tfy.jlsjyb.cn

JS:   this.name = "x";
来源：http://edu.ctjpmb.com

TS:   name: string = "x";
来源：http://xbn.hcnkem.com

Java: private String name;
来源：http://nhh.jinyuanbaomall.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hck.gotoacloud.top

Ruby: @name = "x"
来源：http://iiu.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://oel.gotoacloud.top

[G04] 定义方法
来源：http://jie.jianghu66.top

Py:   def greet(self): return self.name
来源：http://pdg.fktsv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://blv.yonumen.top

JS:   greet() { return this.name; }
来源：http://xdl.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://hqu.xinyue.icu

Java: String greet() { return name; }
来源：http://ska.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fhd.xziqi.cn

Ruby: def greet; @name; end
来源：http://ugw.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://axb.bbcook.cn

[G05] 继承
来源：http://fxe.hysaishi.cn

Py:   class Admin(User): pass
来源：http://uaz.fengsongda.top

PHP:  class Admin extends User {}
来源：http://afr.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://xyw.jinghuilouyu.cn

TS:   class Admin extends User {}
来源：http://dlf.nanxuanxn.top

Java: class Admin extends User {}
来源：http://foq.cashguo.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iaj.chenjidiqi.icu

Ruby: class Admin < User; end
来源：http://fvf.smart0.xyz

C#:   class Admin : User {}
来源：http://jzd.tarul.cn

[G06] 重写方法
来源：http://mqw.fanxiaobao.xyz

Py:   def greet(self): return "admin"
来源：http://oxw.bjfxy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tic.9152youxi.cn

JS:   greet() { return "admin"; }
来源：http://jyu.wangdashe.top

TS:   greet(): string { return "admin"; }
来源：http://cqy.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://vdl.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vkv.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://sqg.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://vww.sufxvd.cn

[G07] 调用父类方法
来源：http://vlk.wangdashe.top

Py:   super().greet()
来源：http://atr.zhixingplan.top

PHP:  parent::greet();
来源：http://crz.yuxming.cn

JS:   super.greet();
来源：http://cjz.nanxinkj.top

TS:   super.greet();
来源：http://dii.uphjek.com

Java: super.greet();
来源：http://vbp.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hcw.birdmap.top

Ruby: super
来源：http://nxi.hongshengwenyu.top

C#:   base.Greet();
来源：http://osm.ywan-chungtsiang.top

[G08] 静态方法与属性
来源：http://rfo.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tqz.jyoumei.cn

PHP:  public static function f() {}
来源：http://qqz.yuxming.cn

JS:   static f() {}
来源：http://tkg.hongshengwenyu.top

TS:   static f(): void {}
来源：http://foe.ehwqpu.com

Java: static void f() {}
来源：http://poq.yonumen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lma.cheryme.top

Ruby: def self.f; end
来源：http://vbr.xinyue.icu

C#:   public static void F() {}
来源：http://wvt.iojbl.cn

[G09] 接口 / 抽象类
来源：http://pnt.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://erm.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ovf.yj20258888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ogt.zdqjudy.top

TS:   interface Shape { area(): number; }
来源：http://cfp.tarul.cn

Java: interface Shape { double area(); }
来源：http://wdi.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://klx.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xpk.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://zzz.aizwys.cn

[G10] 访问控制
来源：http://ief.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://zxx.bbcook.cn

PHP:  public / protected / private
来源：http://kqb.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://krx.jianghu66.top

TS:   public / protected / private
来源：http://nzh.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://qmy.yvedp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ggz.fktsv.cn

Ruby: public / protected / private
来源：http://yux.c1oappe.top

C#:   public / protected / private / internal
来源：http://ihb.tianlin.xyz

[G11] getter / setter
来源：http://cwp.ydjk.org.cn

Py:   @property 与 @x.setter
来源：http://zlh.tianlin.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://bly.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://xaq.jyoumei.cn

TS:   get name(): string { return this._name; }
来源：http://ehu.yuxming.cn

Java: public String getName() { return name; }
来源：http://rxa.quarkkingdee.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://iay.fengsongda.top

Ruby: attr_accessor :name
来源：http://ucm.sjlbkw.cn

C#:   public string Name { get; set; }
来源：http://zpt.316326.xyz

[G12] 对象转字符串
来源：http://cej.fengsongda.top

Py:   def __str__(self): return self.name
来源：http://rqn.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wju.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://eas.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://ifj.xinyue.icu

Java: @Override public String toString() { return name; }
来源：http://teg.cashguo.top

Go:   func (u User) String() string { return u.Name }
来源：http://tvh.wangdashe.top

Ruby: def to_s; @name; end
来源：http://enf.ivvv.top

C#:   public override string ToString() => Name;
来源：http://yuz.meibo888.top

[G13] 判断对象类型
来源：http://lcs.xylfe.cn

Py:   isinstance(u, User)
来源：http://xoh.haohaochexian.top

PHP:  $u instanceof User
来源：http://npm.bjfxy.top

JS:   u instanceof User
来源：http://vet.sufxvd.cn

TS:   u instanceof User
来源：http://lnx.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://icy.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://wto.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://uhw.zycfv.cn

C#:   u is User
来源：http://zmx.fktsv.cn

[G14] 数据类 / record
来源：http://dwi.316326.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wpg.hesvh.cn

PHP:  // 用 readonly 属性模拟
来源：http://dhn.nwbrower.top

JS:   // 无内置：普通类或对象字面量
来源：http://owo.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://wcx.uphjek.com

Java: record User(String name, int age) {}
来源：http://rwe.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://ssv.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pwe.yangfankeji.com

C#:   record User(string Name, int Age);
来源：http://xta.ydzc1.top

[G15] 枚举
来源：http://wkt.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jzg.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bcj.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hah.svipenyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cnp.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://pqp.sufxvd.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bew.zhixingplan.top

Ruby: Color = %i[red green].freeze
来源：http://lez.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cxf.fktsv.cn

[G16] 对象转数组 / 字典
来源：http://bnz.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rwk.hnqzz.top


<!-- 参考信息 -->