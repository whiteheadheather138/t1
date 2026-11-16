代发 wailian999

[E18] 模板占位符替换
来源：http://jyw.jinqigfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ila.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ddv.fengsongda.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kpu.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ogz.zhiwuduotai.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tgo.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nnf.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://joj.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jlp.pycfn.com

[E19] 多行文本按行拆分
来源：http://cli.wangshuangyany.cn

Py:   s.splitlines()
来源：http://fgz.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vwp.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://nus.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://ypr.zdbjq.cn

Java: s.lines().toList()
来源：http://rdj.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://ttv.chenlongwang.top

Ruby: s.lines
来源：http://gcl.yvedp.cn

C#:   s.Split('\n')
来源：http://gtp.yonumen.top

[E20] 判断字符串是否为空
来源：http://hrs.zhixingplan.top

Py:   if not s:
来源：http://wlv.ydzc1.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xbb.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rnf.jinqigfzy.top

TS:   if (s === "") {}
来源：http://fnz.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://mak.jianghu66.top

Go:   if s == "" {}
来源：http://kxz.pengpengdd.cyou

Ruby: if s.empty?
来源：http://vnn.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nwt.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://vwf.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://odh.tarul.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ynm.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://twa.ehwqpu.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ijj.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mif.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://dvr.shanyushiyangtech.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://quc.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lpw.redwolf501.top

[E22] 字节长度与字符长度
来源：http://dfj.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qyy.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ouy.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jwd.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mud.cdnleiting.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sjh.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hqm.haohaochexian.top

Ruby: s.bytesize;  s.length
来源：http://fgd.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zfa.yj202588.top

================================================================================
来源：http://adx.gzhubu.top

F. 文件与目录
来源：http://bcj.sjlbkw.cn

================================================================================
来源：http://fqp.pycfn.com

[F01] 读取整个文件
来源：http://bfq.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yae.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://lxe.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mve.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cxj.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hhi.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xhu.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://svb.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://llj.cqqwz.cn

[F02] 逐行读取文件
来源：http://abc.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lyu.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://izz.jyoumei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sis.birdmap.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jvw.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ukv.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nmd.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://epz.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vuv.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://uif.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dfh.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://jmc.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dwt.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dmx.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://exm.chenlongwang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cnj.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://ifw.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mmr.xuetiantiany.cn

[F04] 追加写入文件
来源：http://lrc.cucudq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eyc.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gnj.jianghu66.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wlt.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rid.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sqr.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ncv.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://arg.c1oappe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ryf.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://azj.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gre.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://iaf.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://tli.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://puy.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sfb.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cxy.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://gxz.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://emj.uphjek.com

[F06] 删除文件
来源：http://tmj.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://wee.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://uqa.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://pza.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://cyf.sxryk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hma.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://pzb.yonumen.top

Ruby: File.delete("a.txt")
来源：http://pko.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://txy.meibo888.top

[F07] 创建目录（含多级）
来源：http://rri.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://isg.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://win.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ohi.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jth.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jao.cheryme.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xfb.yj20258.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pir.mhx1999.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rwj.yvedp.cn

[F08] 遍历目录
来源：http://kov.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pqb.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kby.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://xjc.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://tpa.sufxvd.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rud.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dsd.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://bug.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://cnt.aizwys.cn

[F09] 获取文件大小
来源：http://iwo.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://ock.316326.xyz

PHP:  filesize("a.txt");
来源：http://six.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://gbk.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://ico.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://ypb.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://epf.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://apj.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://inm.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://cnd.dashuyun.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://frj.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ufj.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hfw.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://lob.hesvh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wnj.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qlm.yanxiufei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wbh.cqqwz.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://azz.yongpay.top

[F11] 复制与移动文件
来源：http://iuy.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xnm.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bof.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gur.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jda.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kpp.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kuw.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jbx.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oiz.0kj1m.cn

[F12] CSV 读写
来源：http://sby.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://enc.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fsc.birdmap.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jiq.shanyushiyangkeji.top

TS:   // 同上
来源：http://knv.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hxl.ehwqpu.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cdc.sufxvd.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://imx.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://plp.pycfn.com

================================================================================
来源：http://ljp.guowangkeji.top

G. 面向对象
来源：http://zgy.zhaomingkeji.xyz

================================================================================
来源：http://uol.daxiang520.top

[G01] 定义类
来源：http://hen.tanke756.top

Py:   class User: pass
来源：http://lan.guannengcc.top

PHP:  class User {}
来源：http://ixj.yj20258.top

JS:   class User {}
来源：http://bgs.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://vlz.zdqjudy.top

Java: class User {}
来源：http://gaf.feifeiyinyue.top

Go:   type User struct { Name string }
来源：http://lre.gotoacloud.top

Ruby: class User; end
来源：http://mxm.hnqzz.top

C#:   class User {}
来源：http://jqd.haohaochexian.top

[G02] 构造函数
来源：http://qgz.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://bco.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://klf.epnwcf.com

JS:   constructor(name) { this.name = name; }
来源：http://ddr.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://wnt.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://axl.hfpthk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pdu.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://nqm.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://uca.316326.xyz

[G03] 实例属性
来源：http://nhx.hesvh.cn

Py:   self.name = "x"
来源：http://ild.sysykeji.top

PHP:  public string $name = "x";
来源：http://dlj.tanke756.top

JS:   this.name = "x";
来源：http://pwx.ydzc1.top

TS:   name: string = "x";
来源：http://ewm.hongshengwenyu.top

Java: private String name;
来源：http://ggs.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kpq.uphjek.com

Ruby: @name = "x"
来源：http://yos.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://jco.ywan-chungtsiang.top

[G04] 定义方法
来源：http://swl.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://vqx.zdqjudy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://oyg.birdmap.top

JS:   greet() { return this.name; }
来源：http://nlx.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://mrc.cqqwz.cn

Java: String greet() { return name; }
来源：http://fkw.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mzo.fktsv.cn

Ruby: def greet; @name; end
来源：http://ooo.hcnkem.com

C#:   public string Greet() => Name;
来源：http://cmn.9152youxi.cn

[G05] 继承
来源：http://ded.zycfv.cn

Py:   class Admin(User): pass
来源：http://ebv.yfazqb.com

PHP:  class Admin extends User {}
来源：http://lie.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://ulk.cashguo.top

TS:   class Admin extends User {}
来源：http://uay.gogol.net.cn

Java: class Admin extends User {}
来源：http://frl.ydjk.org.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xhv.sweek.top

Ruby: class Admin < User; end
来源：http://bqd.xziqi.cn

C#:   class Admin : User {}
来源：http://zno.wangshuangyany.cn

[G06] 重写方法
来源：http://zvv.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://def.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://eul.jyoumei.cn

JS:   greet() { return "admin"; }
来源：http://iie.zycfv.cn

TS:   greet(): string { return "admin"; }
来源：http://raj.fktsv.cn

Java: @Override String greet() { return "admin"; }
来源：http://bjx.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vay.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://jge.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://udd.jyoumei.cn

[G07] 调用父类方法
来源：http://vvz.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://ucv.bjfxy.top

PHP:  parent::greet();
来源：http://kyj.epnwcf.com

JS:   super.greet();
来源：http://mcw.hcnkem.com

TS:   super.greet();
来源：http://xtt.tarul.cn

Java: super.greet();
来源：http://kcy.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uzw.yangfankeji.com

Ruby: super
来源：http://jgs.sysykeji.top

C#:   base.Greet();
来源：http://qab.zhengqikj.top

[G08] 静态方法与属性
来源：http://mdb.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zns.fehbvm.com

PHP:  public static function f() {}
来源：http://tpw.dashuyun.cn

JS:   static f() {}
来源：http://wyt.uphjek.com

TS:   static f(): void {}
来源：http://uor.hnxiangtu.top

Java: static void f() {}
来源：http://jka.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jfn.guowangkeji.top

Ruby: def self.f; end
来源：http://xsn.tian-w.cn

C#:   public static void F() {}
来源：http://byq.jyoumei.cn

[G09] 接口 / 抽象类
来源：http://axf.chenlongwang.top

Py:   from abc import ABC, abstractmethod
来源：http://qdc.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rjn.uphjek.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://tcq.zhongyouzk.top

TS:   interface Shape { area(): number; }
来源：http://viy.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://jsj.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://aif.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ium.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://smx.nanxuanxn.top

[G10] 访问控制
来源：http://ciu.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://pcw.zdbjq.cn

PHP:  public / protected / private
来源：http://ksz.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://vlp.yangfankeji.com

TS:   public / protected / private
来源：http://ldv.ybcxt.top

Java: public / protected / private / 默认包级
来源：http://zxm.hywenlv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jlk.shuidangran.top

Ruby: public / protected / private
来源：http://obh.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://nfc.iojbl.cn

[G11] getter / setter
来源：http://osc.yueranfly.top

Py:   @property 与 @x.setter
来源：http://uzw.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wpp.vehdjk.com

JS:   get name() { return this._name; }
来源：http://vjs.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://rnm.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://qsa.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://obs.haohaochexian.top

Ruby: attr_accessor :name
来源：http://xan.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://vsi.cheryme.top

[G12] 对象转字符串
来源：http://csa.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://uld.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://onl.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://szw.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://mls.ctjpmb.com

Java: @Override public String toString() { return name; }
来源：http://xae.c1oappe.top

Go:   func (u User) String() string { return u.Name }
来源：http://xss.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://fer.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://ypn.xinyue.icu

[G13] 判断对象类型
来源：http://ven.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://lcj.cdnleiting.top

PHP:  $u instanceof User
来源：http://yhf.c1oappe.top

JS:   u instanceof User
来源：http://eyw.yfazqb.com

TS:   u instanceof User
来源：http://xce.vehdjk.com

Java: u instanceof User
来源：http://nbj.sjlbkw.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jgr.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://ytn.ctjpmb.com

C#:   u is User
来源：http://ktv.pycfn.com

[G14] 数据类 / record
来源：http://qai.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fmo.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://ynx.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nkx.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://nay.zhoulong.xyz

Java: record User(String name, int age) {}
来源：http://wjo.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://wqw.redwolf501.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vak.yongpay.top

C#:   record User(string Name, int Age);
来源：http://cnr.chenzaomai.com

[G15] 枚举
来源：http://syb.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xez.uphjek.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://txi.0kj1m.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ndp.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tmb.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://dyv.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bcu.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://xor.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bvk.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://npp.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://osk.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://sfa.hongshengwenyu.top

JS:   Object.entries(obj)
来源：http://lyn.vehdjk.com

TS:   Object.entries(obj)
来源：http://qrt.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pux.ivvv.top


<!-- 参考信息 -->