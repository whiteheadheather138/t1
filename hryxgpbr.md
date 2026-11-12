代发 wailian999

[E18] 模板占位符替换
来源：http://tau.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kmy.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ylz.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://yvj.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mqz.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://doy.gogol.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kau.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ipm.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kjz.yangfankeji.com

[E19] 多行文本按行拆分
来源：http://nyf.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://lqc.iojbl.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://szh.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://gof.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://mle.tanke756.top

Java: s.lines().toList()
来源：http://xzy.shanyushiyangtech.top

Go:   strings.Split(s, "\n")
来源：http://ndn.cdnleiting.top

Ruby: s.lines
来源：http://wnf.cheryme.top

C#:   s.Split('\n')
来源：http://mnj.smart0.xyz

[E20] 判断字符串是否为空
来源：http://kya.vqdsnc.cn

Py:   if not s:
来源：http://fdx.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vvr.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://drl.zycfv.cn

TS:   if (s === "") {}
来源：http://arl.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://rlg.guowangkeji.top

Go:   if s == "" {}
来源：http://ukg.zhengqikj.top

Ruby: if s.empty?
来源：http://adn.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yca.uphjek.com

[E21] 超长截断加省略号
来源：http://feq.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qku.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dhl.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nde.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jdy.zhijiandao.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jsq.hongshengwenyu.top

Go:   // 按 rune 判断长度后截断
来源：http://ibl.nanxuanxn.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qoo.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cpe.yonumen.top

[E22] 字节长度与字符长度
来源：http://ymz.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cdt.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://taz.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wma.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pnd.chenlongwang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://phx.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lii.zhoulong.xyz

Ruby: s.bytesize;  s.length
来源：http://wqk.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pqj.hcnkem.com

================================================================================
来源：http://orv.ctjpmb.com

F. 文件与目录
来源：http://zcm.chenlongwang.top

================================================================================
来源：http://tfw.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://thj.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yvx.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://stp.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uvb.smart0.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wlw.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qcx.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sqz.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://onk.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://xll.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://hwe.9152youxi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://afs.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dvm.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jhf.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mzz.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eig.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://otg.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ukp.zhaomingkeji.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zsz.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://lsv.hnxiangtu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://brd.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tdf.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ohi.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://anw.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mmo.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kpx.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://yxp.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cfz.guannengcc.top

[F04] 追加写入文件
来源：http://xdd.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mbh.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qtc.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dap.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uoi.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xbk.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kev.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ngb.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://egh.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://eor.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rqi.pycfn.com

PHP:  file_exists("a.txt");
来源：http://xuu.dashuyun.cn

JS:   fs.existsSync("a.txt")
来源：http://xme.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://uwc.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://asp.yj20258888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sqy.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://czc.hammf.cn

C#:   File.Exists("a.txt")
来源：http://bni.jinqigufen.top

[F06] 删除文件
来源：http://xvb.guannengcc.top

Py:   os.remove("a.txt")
来源：http://mmk.gzhubu.top

PHP:  unlink("a.txt");
来源：http://sdt.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://ltn.fktsv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vcw.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mpc.yonumen.top

Go:   os.Remove("a.txt")
来源：http://hcw.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://ozn.ywan-chungtsiang.top

C#:   File.Delete("a.txt");
来源：http://irg.hesvh.cn

[F07] 创建目录（含多级）
来源：http://sre.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zhx.bjfxy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://goq.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yry.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eex.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ukc.cheryme.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rav.jqgfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://goy.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mce.fengsongda.top

[F08] 遍历目录
来源：http://ldz.fanxiaobao.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://fuh.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qux.zhiwuduotai.top

JS:   fs.readdirSync("dir")
来源：http://rhm.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://eyq.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ylz.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ykk.0kj1m.cn

Ruby: Dir.children("dir")
来源：http://yjl.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://gzs.zycfv.cn

[F09] 获取文件大小
来源：http://twq.vehdjk.com

Py:   os.path.getsize("a.txt")
来源：http://mai.gaohongyu789.top

PHP:  filesize("a.txt");
来源：http://opt.xziqi.cn

JS:   fs.statSync("a.txt").size
来源：http://lzr.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://lzn.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tbu.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://moa.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://owe.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://rch.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://sqt.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dda.jinqigfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://twa.jinqigufen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lkk.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://ifu.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rnb.xziqi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://klj.yj20258888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ivh.fktsv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://htr.svipenyu.cn

[F11] 复制与移动文件
来源：http://voj.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://slq.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tpk.yongpay.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://top.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rnr.epnwcf.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://saq.hammf.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sse.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mbf.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jte.xuanzx.com

[F12] CSV 读写
来源：http://adh.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oaw.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wnn.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pbt.fanxiaobao.xyz

TS:   // 同上
来源：http://kkz.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iut.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://neu.jinqigfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qel.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wmy.fengsongda.top

================================================================================
来源：http://lab.hnxiangtu.top

G. 面向对象
来源：http://hqq.fktsv.cn

================================================================================
来源：http://zfo.zhiwuduotai.top

[G01] 定义类
来源：http://jha.gzhubu.top

Py:   class User: pass
来源：http://dle.tianlin.xyz

PHP:  class User {}
来源：http://rgp.yj20258.top

JS:   class User {}
来源：http://tfk.chenlongwang.top

TS:   class User { name: string = ""; }
来源：http://pkm.fengsongda.top

Java: class User {}
来源：http://tws.guannengcc.top

Go:   type User struct { Name string }
来源：http://dqy.zhoulong.xyz

Ruby: class User; end
来源：http://dwv.sysykeji.top

C#:   class User {}
来源：http://lbq.fzhhl.top

[G02] 构造函数
来源：http://hwo.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://ijk.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://klv.shanyushiyangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://xch.9152youxi.cn

TS:   constructor(public name: string) {}
来源：http://qgy.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://lop.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eqk.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://ljp.tian-w.cn

C#:   public User(string name) { Name = name; }
来源：http://mtn.sweek.top

[G03] 实例属性
来源：http://xsl.jlsjyb.cn

Py:   self.name = "x"
来源：http://yzj.xylfe.cn

PHP:  public string $name = "x";
来源：http://zqq.tianlin.xyz

JS:   this.name = "x";
来源：http://qhh.shanyushiyangtech.top

TS:   name: string = "x";
来源：http://kef.hfpthk.cn

Java: private String name;
来源：http://ffb.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aod.chenzaomai.com

Ruby: @name = "x"
来源：http://tqx.zdbjq.cn

C#:   public string Name { get; set; } = "x";
来源：http://xhc.haohaochexian.top

[G04] 定义方法
来源：http://soc.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://scf.gotoacloud.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uxv.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://jum.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://lui.nwbrower.top

Java: String greet() { return name; }
来源：http://wpc.9152youxi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nbm.yuanzhike.top

Ruby: def greet; @name; end
来源：http://jsx.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://wdy.ivvv.top

[G05] 继承
来源：http://ujx.fktsv.cn

Py:   class Admin(User): pass
来源：http://ema.hfpthk.cn

PHP:  class Admin extends User {}
来源：http://nkq.jyoumei.cn

JS:   class Admin extends User {}
来源：http://xmi.gzhubu.top

TS:   class Admin extends User {}
来源：http://zdc.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://asy.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ycl.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://xmg.hcnkem.com

C#:   class Admin : User {}
来源：http://lkg.zycfv.cn

[G06] 重写方法
来源：http://opp.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://uiq.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rua.ehwqpu.com

JS:   greet() { return "admin"; }
来源：http://cip.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://cxr.yuxming.cn

Java: @Override String greet() { return "admin"; }
来源：http://egg.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fmk.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://wzf.aizwys.cn

C#:   public override string Greet() => "admin";
来源：http://xwv.vehdjk.com

[G07] 调用父类方法
来源：http://woc.shuidangran.top

Py:   super().greet()
来源：http://dxe.zhijiandao.cn

PHP:  parent::greet();
来源：http://nnq.wangshuangyany.cn

JS:   super.greet();
来源：http://kbm.pengpengdd.cyou

TS:   super.greet();
来源：http://ovv.xylfe.cn

Java: super.greet();
来源：http://fqy.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://arq.hnqzz.top

Ruby: super
来源：http://slz.pycfn.com

C#:   base.Greet();
来源：http://txr.hcnkem.com

[G08] 静态方法与属性
来源：http://nxf.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ihh.birdmap.top

PHP:  public static function f() {}
来源：http://bzh.dianchejie.cn

JS:   static f() {}
来源：http://syd.yuanzhike.top

TS:   static f(): void {}
来源：http://jbq.pycfn.com

Java: static void f() {}
来源：http://uyk.tanke756.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vdm.tianlin.xyz

Ruby: def self.f; end
来源：http://afm.gotoacloud.top

C#:   public static void F() {}
来源：http://fus.fehbvm.com

[G09] 接口 / 抽象类
来源：http://rqy.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://naw.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://xzq.sweek.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jqd.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://ioo.tarul.cn

Java: interface Shape { double area(); }
来源：http://ubc.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://fuo.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qjj.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://iaq.316326.xyz

[G10] 访问控制
来源：http://vpx.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://acm.jinyuanbaomall.cn

PHP:  public / protected / private
来源：http://lqm.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://akl.smart0.xyz

TS:   public / protected / private
来源：http://cyj.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://tou.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nla.chenlongwang.top

Ruby: public / protected / private
来源：http://jbf.sysykeji.top

C#:   public / protected / private / internal
来源：http://qho.zdqjudy.top

[G11] getter / setter
来源：http://cqi.xylfe.cn

Py:   @property 与 @x.setter
来源：http://onx.jyoumei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fii.xylfe.cn

JS:   get name() { return this._name; }
来源：http://xdw.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://ygm.iojbl.cn

Java: public String getName() { return name; }
来源：http://yjg.quarkkingdee.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fef.mhx1999.top

Ruby: attr_accessor :name
来源：http://ttk.iojbl.cn

C#:   public string Name { get; set; }
来源：http://sqk.uphjek.com

[G12] 对象转字符串
来源：http://gwv.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://rtn.epnwcf.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://tcn.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://nbk.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://wja.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://ilw.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://zob.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://kqk.haohaochexian.top

C#:   public override string ToString() => Name;
来源：http://egm.jiagoushi.top

[G13] 判断对象类型
来源：http://nbj.sufxvd.cn

Py:   isinstance(u, User)
来源：http://vqj.yj20258888.top

PHP:  $u instanceof User
来源：http://jpd.redwolf501.top

JS:   u instanceof User
来源：http://sfy.bbcook.cn

TS:   u instanceof User
来源：http://itt.guowangkeji.top

Java: u instanceof User
来源：http://ids.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ond.tarul.cn

Ruby: u.is_a?(User)
来源：http://ner.jqgufenzy.top

C#:   u is User
来源：http://zkg.xuetiantiany.cn

[G14] 数据类 / record
来源：http://kpa.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mxf.nanxuanxn.top

PHP:  // 用 readonly 属性模拟
来源：http://xks.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://mta.bbcook.cn

TS:   type User = { name: string; age: number };
来源：http://tdm.xziqi.cn

Java: record User(String name, int age) {}
来源：http://hqp.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://lyz.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mcd.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://wrk.shangyingyoupin.top

[G15] 枚举
来源：http://usj.jiagoushi.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://efr.cucudq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kev.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://isi.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ncj.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://ipe.sysykeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cdb.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://fha.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ive.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://jgg.yongpay.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xti.tarul.cn

PHP:  get_object_vars($obj);
来源：http://pdr.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://bvi.dashuyun.cn

TS:   Object.entries(obj)
来源：http://ofw.cucudq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bhv.hywenlv.cn


<!-- 参考信息 -->