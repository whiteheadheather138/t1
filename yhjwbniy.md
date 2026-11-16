代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nkt.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ypw.guowangkeji.top

Ruby: s.capitalize
来源：http://eod.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dgh.iojbl.cn

[E18] 模板占位符替换
来源：http://fam.tian-w.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wvy.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lps.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://xck.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://ipw.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vjr.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hqe.yongpay.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cqs.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xjy.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://hht.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://axy.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ygv.yj20258.top

JS:   s.split(/\r?\n/)
来源：http://fve.fehbvm.com

TS:   s.split(/\r?\n/)
来源：http://vlx.epnwcf.com

Java: s.lines().toList()
来源：http://oye.uphjek.com

Go:   strings.Split(s, "\n")
来源：http://mdx.yfazqb.com

Ruby: s.lines
来源：http://nrg.fehbvm.com

C#:   s.Split('\n')
来源：http://htg.yuxming.cn

[E20] 判断字符串是否为空
来源：http://bvw.hongshengwenyu.top

Py:   if not s:
来源：http://foc.gzhubu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lnk.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://spz.dashuyun.cn

TS:   if (s === "") {}
来源：http://acr.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://ogv.feifeiyinyue.top

Go:   if s == "" {}
来源：http://qzi.andypj.xyz

Ruby: if s.empty?
来源：http://gbh.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aew.bjfxy.top

[E21] 超长截断加省略号
来源：http://jgl.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wfb.tian-w.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qlq.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yln.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fup.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://suv.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://day.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ufq.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gig.yonumen.top

[E22] 字节长度与字符长度
来源：http://igs.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rae.nwbrower.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qwv.yanxiufei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ypx.0kj1m.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wrg.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hpv.zhaomingkeji.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://glp.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://lzg.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xzf.pycfn.com

================================================================================
来源：http://hvb.pycfn.com

F. 文件与目录
来源：http://aza.aizwys.cn

================================================================================
来源：http://nde.uphjek.com

[F01] 读取整个文件
来源：http://hoj.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ewl.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://uqz.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cck.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ujg.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://exh.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gew.wangshuangyany.cn

Ruby: File.read("a.txt")
来源：http://adx.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://eik.tanke756.top

[F02] 逐行读取文件
来源：http://ghr.xinyue.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pax.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bys.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nfk.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rcg.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wuj.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qww.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cil.ehwqpu.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gda.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://fty.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yuj.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://avm.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ubj.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pup.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kxy.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xlf.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://mog.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jgx.gzhubu.top

[F04] 追加写入文件
来源：http://jrg.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://avu.sweek.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gfv.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ayj.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pkp.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rxj.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rux.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kmk.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xml.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://mth.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mwm.hammf.cn

PHP:  file_exists("a.txt");
来源：http://ucw.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://ahf.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://aej.fanxiaobao.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://imb.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://klo.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://boj.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://cjt.yj20258888.top

[F06] 删除文件
来源：http://mxp.shuidangran.top

Py:   os.remove("a.txt")
来源：http://vfn.9152youxi.cn

PHP:  unlink("a.txt");
来源：http://jao.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rhe.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://etq.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sdf.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://sbf.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://uhw.birdmap.top

C#:   File.Delete("a.txt");
来源：http://pfu.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://soq.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qoi.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://omn.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mgx.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gir.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dbq.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xhy.yj20258888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mja.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qqn.wangdashe.top

[F08] 遍历目录
来源：http://srh.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ndi.wangshuangyany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://viv.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://dqb.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://xbz.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xuo.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://czk.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://xoa.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://drh.mhx1999.top

[F09] 获取文件大小
来源：http://smd.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://pzr.yfazqb.com

PHP:  filesize("a.txt");
来源：http://khk.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://niz.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://hac.xuanzx.com

Java: Files.size(Path.of("a.txt"))
来源：http://hxx.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zhh.yj20258888.top

Ruby: File.size("a.txt")
来源：http://fsm.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://gpo.fengsongda.top

[F10] 取文件扩展名 / 文件名
来源：http://jxp.yj20258.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yva.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lbi.hfpthk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gvd.smart0.xyz

TS:   path.extname("a.txt")
来源：http://ibg.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bep.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fuo.hcnkem.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xbj.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xea.guowangkeji.top

[F11] 复制与移动文件
来源：http://bcj.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nlw.fzhhl.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lny.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://onq.zhongyouzk.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jkx.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qpz.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wcg.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lhm.chenlongwang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vrs.c1oappe.top

[F12] CSV 读写
来源：http://ihv.jlsjyb.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gwv.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gvk.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ftn.yfazqb.com

TS:   // 同上
来源：http://bui.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mak.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gdp.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tem.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yhl.wangshuangyany.cn

================================================================================
来源：http://pqk.zhaomingkeji.xyz

G. 面向对象
来源：http://smn.guowangkeji.top

================================================================================
来源：http://rwr.yanxiufei.cn

[G01] 定义类
来源：http://rmq.yj20258.top

Py:   class User: pass
来源：http://qsl.aizwys.cn

PHP:  class User {}
来源：http://ooo.cheryme.top

JS:   class User {}
来源：http://uzr.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://cbv.yfazqb.com

Java: class User {}
来源：http://juh.jiagoushi.top

Go:   type User struct { Name string }
来源：http://spv.zdqjudy.top

Ruby: class User; end
来源：http://wfa.jianghu66.top

C#:   class User {}
来源：http://yvw.ehwqpu.com

[G02] 构造函数
来源：http://aoz.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://xff.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ckt.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://njn.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://xwt.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://hkc.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://see.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://gfe.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://pfv.svipenyu.cn

[G03] 实例属性
来源：http://qtz.chenzaomai.com

Py:   self.name = "x"
来源：http://zbe.guannengcc.top

PHP:  public string $name = "x";
来源：http://hzu.pycfn.com

JS:   this.name = "x";
来源：http://ezj.uphjek.com

TS:   name: string = "x";
来源：http://eud.hywenlv.cn

Java: private String name;
来源：http://vrj.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vvf.daria6918.cn

Ruby: @name = "x"
来源：http://kqe.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://vnu.hnqzz.top

[G04] 定义方法
来源：http://amj.daxiang520.top

Py:   def greet(self): return self.name
来源：http://iug.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://iur.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://rfh.hysaishi.cn

TS:   greet(): string { return this.name; }
来源：http://vep.aibaodan.cn

Java: String greet() { return name; }
来源：http://lkx.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://nra.xuetiantiany.cn

Ruby: def greet; @name; end
来源：http://eju.jianghu66.top

C#:   public string Greet() => Name;
来源：http://clt.cucudq.cn

[G05] 继承
来源：http://fpo.shuidangran.top

Py:   class Admin(User): pass
来源：http://tne.yfazqb.com

PHP:  class Admin extends User {}
来源：http://gsc.cashguo.top

JS:   class Admin extends User {}
来源：http://dgg.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://hlj.yj20258.top

Java: class Admin extends User {}
来源：http://dew.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://utl.dianchejie.cn

Ruby: class Admin < User; end
来源：http://gja.cdnleiting.top

C#:   class Admin : User {}
来源：http://xbg.gaohongyu789.top

[G06] 重写方法
来源：http://wts.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://mno.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kav.birdmap.top

JS:   greet() { return "admin"; }
来源：http://maw.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://aqh.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://qey.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mvr.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://svw.zhixingplan.top

C#:   public override string Greet() => "admin";
来源：http://cza.daria6918.cn

[G07] 调用父类方法
来源：http://fxa.zhixingplan.top

Py:   super().greet()
来源：http://scd.jinqigfzy.top

PHP:  parent::greet();
来源：http://gdd.bbcook.cn

JS:   super.greet();
来源：http://nff.snrcjt.cn

TS:   super.greet();
来源：http://mth.jinyuanbaomall.cn

Java: super.greet();
来源：http://hrz.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jqt.uphjek.com

Ruby: super
来源：http://qcc.xuetiantiany.cn

C#:   base.Greet();
来源：http://gbp.gotoacloud.top

[G08] 静态方法与属性
来源：http://kov.snrcjt.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sip.epnwcf.com

PHP:  public static function f() {}
来源：http://zap.jqgufenzy.top

JS:   static f() {}
来源：http://pmt.ydzc1.top

TS:   static f(): void {}
来源：http://bdo.zdqjudy.top

Java: static void f() {}
来源：http://qtz.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tgh.chenlongwang.top

Ruby: def self.f; end
来源：http://xjn.tarul.cn

C#:   public static void F() {}
来源：http://yrv.aizwys.cn

[G09] 接口 / 抽象类
来源：http://ona.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://nsh.haohaochexian.top

PHP:  interface Shape { public function area(): float; }
来源：http://rqm.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qxf.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://gze.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://rau.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://efj.hnqzz.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cfg.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://hyu.zdqjudy.top

[G10] 访问控制
来源：http://zyb.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://wgw.hnqzz.top

PHP:  public / protected / private
来源：http://gcu.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://oqg.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://oys.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://xwf.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kum.uphjek.com

Ruby: public / protected / private
来源：http://uaa.xuanzx.com

C#:   public / protected / private / internal
来源：http://nat.yfazqb.com

[G11] getter / setter
来源：http://lrd.smart0.xyz

Py:   @property 与 @x.setter
来源：http://nym.cheryme.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ipy.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://npx.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://wot.0kj1m.cn

Java: public String getName() { return name; }
来源：http://tqw.zhongyouzk.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xdm.hysaishi.cn

Ruby: attr_accessor :name
来源：http://btx.yueranfly.top

C#:   public string Name { get; set; }
来源：http://abd.tanke756.top

[G12] 对象转字符串
来源：http://sic.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://erj.nanxuanxn.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vnj.bjfxy.top

JS:   toString() { return this.name; }
来源：http://nks.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://bkw.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://eyz.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://his.tanke756.top

Ruby: def to_s; @name; end
来源：http://mdb.meibo888.top

C#:   public override string ToString() => Name;
来源：http://olu.wangdashe.top

[G13] 判断对象类型
来源：http://qre.redwolf501.top

Py:   isinstance(u, User)
来源：http://eok.xingfuxueyuan.xyz

PHP:  $u instanceof User
来源：http://opl.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://mez.hnxiangtu.top

TS:   u instanceof User
来源：http://llm.yongpay.top

Java: u instanceof User
来源：http://qwo.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qbe.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://vvj.chenlongwang.top

C#:   u is User
来源：http://azw.jlsjyb.cn

[G14] 数据类 / record
来源：http://vyf.yj20258888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://brb.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://cga.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://cgy.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://jch.chenzaomai.com

Java: record User(String name, int age) {}
来源：http://zay.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://xaz.hfpthk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hvs.jqgfzy.top

C#:   record User(string Name, int Age);
来源：http://rud.mhx1999.top

[G15] 枚举
来源：http://aaw.ybcxt.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bcx.tanke756.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pfw.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cnj.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fdv.yanxiufei.cn

Java: enum Color { RED, GREEN }
来源：http://snr.cqqwz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lqo.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://uhk.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lbj.shanyushiyangtech.top

[G16] 对象转数组 / 字典
来源：http://yve.cucudq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zdv.316326.xyz


<!-- 参考信息 -->