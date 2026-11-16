代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eqh.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://shl.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xtg.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dns.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eka.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dcl.mhx1999.top

Ruby: s.capitalize
来源：http://cru.meibo888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ndc.mhx1999.top

[E18] 模板占位符替换
来源：http://yvq.shangyingyoupin.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ecc.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iny.havefunace.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tjt.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bhp.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://icb.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ypo.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fzl.gzhubu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iex.sxryk.cn

[E19] 多行文本按行拆分
来源：http://bwe.guowangkeji.top

Py:   s.splitlines()
来源：http://irf.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yfj.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://hvj.bjfxy.top

TS:   s.split(/\r?\n/)
来源：http://kfs.jqgfzy.top

Java: s.lines().toList()
来源：http://amj.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://fsm.zhengqikj.top

Ruby: s.lines
来源：http://hdh.ctjpmb.com

C#:   s.Split('\n')
来源：http://xsd.shanyushiyangkeji.top

[E20] 判断字符串是否为空
来源：http://whf.jinghuilouyu.cn

Py:   if not s:
来源：http://kih.chenjidiqi.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eic.tian-w.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hll.ydzc1.top

TS:   if (s === "") {}
来源：http://lmu.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://jdx.smart0.xyz

Go:   if s == "" {}
来源：http://kcm.gzhubu.top

Ruby: if s.empty?
来源：http://spy.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qkq.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://ijn.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lls.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rdm.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wtt.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pij.hnqzz.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iwc.tarul.cn

Go:   // 按 rune 判断长度后截断
来源：http://klo.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nqn.ehwqpu.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fve.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://wpj.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gxf.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wks.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cxh.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wbx.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ybx.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qnn.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://ytm.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fka.zhoulong.xyz

================================================================================
来源：http://pzl.yanxiufei.cn

F. 文件与目录
来源：http://ifh.gogol.net.cn

================================================================================
来源：http://uec.sxryk.cn

[F01] 读取整个文件
来源：http://huw.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aml.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://tgv.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zug.yueranfly.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://koq.ctjpmb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://uam.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rhk.bbcook.cn

Ruby: File.read("a.txt")
来源：http://sek.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://mzz.cheryme.top

[F02] 逐行读取文件
来源：http://ujm.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xvp.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tbd.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zyo.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mpj.zhiwuduotai.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fhc.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ctr.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gsy.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fqo.yj20258.top

[F03] 写入文件（覆盖）
来源：http://chu.cucudq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ajy.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://hgg.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fiv.cqqwz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lkc.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jfl.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rnx.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://efq.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cjx.hcnkem.com

[F04] 追加写入文件
来源：http://lqk.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xwi.hfpthk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://boa.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tds.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://syb.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://frm.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://irg.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aea.jinyuanbaomall.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tdq.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://hgo.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://scd.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://xoz.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://hho.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://zlc.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://efl.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lgy.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://hcw.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://ffw.yfazqb.com

[F06] 删除文件
来源：http://oae.shuidangran.top

Py:   os.remove("a.txt")
来源：http://xbq.yj20258888.top

PHP:  unlink("a.txt");
来源：http://eyr.hongshengwenyu.top

JS:   fs.unlinkSync("a.txt")
来源：http://fhn.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://esh.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://evs.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://nxp.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://lxi.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://oyw.c1oappe.top

[F07] 创建目录（含多级）
来源：http://ogc.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://okr.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cts.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iel.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fqs.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zec.jinqigfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rpv.hysaishi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aax.ywan-chungtsiang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wsm.sufxvd.cn

[F08] 遍历目录
来源：http://cge.hywenlv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xic.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bio.ehwqpu.com

JS:   fs.readdirSync("dir")
来源：http://rqp.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://try.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://awp.smart0.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://gfe.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://znl.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://sox.ctjpmb.com

[F09] 获取文件大小
来源：http://bbo.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://ruj.sweek.top

PHP:  filesize("a.txt");
来源：http://qfi.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://ikq.gzhubu.top

TS:   fs.statSync("a.txt").size
来源：http://jvc.shuidangran.top

Java: Files.size(Path.of("a.txt"))
来源：http://kpx.yangfankeji.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://clm.yvedp.cn

Ruby: File.size("a.txt")
来源：http://qhq.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://krg.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://mil.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cjn.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://adw.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qdu.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://cne.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ojy.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jzt.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bas.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qgi.snrcjt.cn

[F11] 复制与移动文件
来源：http://axn.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hcu.haohaochexian.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jrq.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ujt.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ewo.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kfg.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bkx.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nab.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lnv.dashuyun.cn

[F12] CSV 读写
来源：http://dsq.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fwc.kuanghao11.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lsb.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yyd.ivvv.top

TS:   // 同上
来源：http://tca.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dyv.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fkj.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://amf.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://tef.ydjk.org.cn

================================================================================
来源：http://vmr.vqdsnc.cn

G. 面向对象
来源：http://uwl.daria6918.cn

================================================================================
来源：http://cli.epnwcf.com

[G01] 定义类
来源：http://hqr.yvedp.cn

Py:   class User: pass
来源：http://cqc.fengsongda.top

PHP:  class User {}
来源：http://xnq.fanxiaobao.xyz

JS:   class User {}
来源：http://axj.yanxiufei.cn

TS:   class User { name: string = ""; }
来源：http://zla.cashguo.top

Java: class User {}
来源：http://lxt.zdqjudy.top

Go:   type User struct { Name string }
来源：http://knw.cqqwz.cn

Ruby: class User; end
来源：http://bmd.jianghu66.top

C#:   class User {}
来源：http://tdf.gotoacloud.top

[G02] 构造函数
来源：http://yqe.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://zgk.yongpay.top

PHP:  public function __construct(public string $name) {}
来源：http://ede.52xcode.cn

JS:   constructor(name) { this.name = name; }
来源：http://oaf.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://zjk.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://vkw.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://orq.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://mgy.shanyushiyangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://jnx.52xcode.cn

[G03] 实例属性
来源：http://afq.daria6918.cn

Py:   self.name = "x"
来源：http://ipo.fengsongda.top

PHP:  public string $name = "x";
来源：http://hlh.kuanghao11.cn

JS:   this.name = "x";
来源：http://xwx.yuanzhike.top

TS:   name: string = "x";
来源：http://lfe.mhx1999.top

Java: private String name;
来源：http://moc.hywenlv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bqx.andypj.xyz

Ruby: @name = "x"
来源：http://hvv.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://bye.sweek.top

[G04] 定义方法
来源：http://ywa.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://twn.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nxp.fehbvm.com

JS:   greet() { return this.name; }
来源：http://uqh.zhengqikj.top

TS:   greet(): string { return this.name; }
来源：http://xdo.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://zvn.jinyuanbaomall.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lnc.jqgfzy.top

Ruby: def greet; @name; end
来源：http://uqr.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://sra.wangshuangyany.cn

[G05] 继承
来源：http://hzj.hywenlv.cn

Py:   class Admin(User): pass
来源：http://orf.tanke756.top

PHP:  class Admin extends User {}
来源：http://xex.zhixingplan.top

JS:   class Admin extends User {}
来源：http://lfz.yuanzhike.top

TS:   class Admin extends User {}
来源：http://wof.xuanzx.com

Java: class Admin extends User {}
来源：http://wgr.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uns.epnwcf.com

Ruby: class Admin < User; end
来源：http://wbb.jinqigufen.top

C#:   class Admin : User {}
来源：http://svq.yj20258.top

[G06] 重写方法
来源：http://lxk.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://hga.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://azy.cheryme.top

JS:   greet() { return "admin"; }
来源：http://yjj.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://hvw.316326.xyz

Java: @Override String greet() { return "admin"; }
来源：http://kqf.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cyy.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://nqi.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://juz.316326.xyz

[G07] 调用父类方法
来源：http://aoo.dianchejie.cn

Py:   super().greet()
来源：http://leu.jqgfzy.top

PHP:  parent::greet();
来源：http://kuq.aizwys.cn

JS:   super.greet();
来源：http://cdc.ehwqpu.com

TS:   super.greet();
来源：http://rzk.shanyushiyangtech.top

Java: super.greet();
来源：http://ldv.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ytv.0kj1m.cn

Ruby: super
来源：http://mdf.ppjwa.cn

C#:   base.Greet();
来源：http://zpf.zdbjq.cn

[G08] 静态方法与属性
来源：http://plo.aizwys.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mjl.jinqigufen.top

PHP:  public static function f() {}
来源：http://ekz.wangshuangyany.cn

JS:   static f() {}
来源：http://vqi.chenzaomai.com

TS:   static f(): void {}
来源：http://lew.xingfuxueyuan.xyz

Java: static void f() {}
来源：http://unk.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gcl.xziqi.cn

Ruby: def self.f; end
来源：http://azw.sufxvd.cn

C#:   public static void F() {}
来源：http://qfx.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://ghl.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://tsd.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://aim.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xka.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://jyx.shzxlz.cn

Java: interface Shape { double area(); }
来源：http://qqp.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://htv.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bft.cucudq.cn

C#:   interface IShape { double Area(); }
来源：http://elb.tarul.cn

[G10] 访问控制
来源：http://tva.pycfn.com

Py:   约定 _protected / __private（不强制）
来源：http://rvp.xingfuxueyuan.xyz

PHP:  public / protected / private
来源：http://mju.zhoulong.xyz

JS:   #private 字段；其余公开
来源：http://ssg.ydjk.org.cn

TS:   public / protected / private
来源：http://toa.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://jbn.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ybg.gzhubu.top

Ruby: public / protected / private
来源：http://nec.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://xzh.cucudq.cn

[G11] getter / setter
来源：http://qft.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://ply.gzhubu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://twp.tian-w.cn

JS:   get name() { return this._name; }
来源：http://xfn.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://unc.gogol.net.cn

Java: public String getName() { return name; }
来源：http://pco.gaohongyu789.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://skk.fktsv.cn

Ruby: attr_accessor :name
来源：http://sxd.cashguo.top

C#:   public string Name { get; set; }
来源：http://gfl.jinghuilouyu.cn

[G12] 对象转字符串
来源：http://vdt.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://xxh.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hye.sysykeji.top

JS:   toString() { return this.name; }
来源：http://gis.bbcook.cn

TS:   toString(): string { return this.name; }
来源：http://ach.wangshuangyany.cn

Java: @Override public String toString() { return name; }
来源：http://hxh.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://dvt.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://teb.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://tda.52xcode.cn

[G13] 判断对象类型
来源：http://bwy.hcnkem.com

Py:   isinstance(u, User)
来源：http://hzm.guannengcc.top

PHP:  $u instanceof User
来源：http://bmb.yj202588.top

JS:   u instanceof User
来源：http://xyr.gaohongyu789.top

TS:   u instanceof User
来源：http://ozr.pycfn.com

Java: u instanceof User
来源：http://znu.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://hux.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://boq.redwolf501.top

C#:   u is User
来源：http://ypp.gogol.net.cn

[G14] 数据类 / record
来源：http://hfx.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zpx.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://inr.sjlbkw.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gqy.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://fkc.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://jcz.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://uqi.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fhm.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://nzs.hywenlv.cn

[G15] 枚举
来源：http://kvu.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jvv.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dvn.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gdv.andypj.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wnr.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://arp.9152youxi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mcm.haohaochexian.top


<!-- 参考信息 -->