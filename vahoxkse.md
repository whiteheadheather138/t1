代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://rom.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dfj.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cxf.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sak.ivvv.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jxk.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://wex.yvedp.cn

Py:   s.splitlines()
来源：http://qoy.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hsx.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://dmt.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://vve.jiagoushi.top

Java: s.lines().toList()
来源：http://lmq.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://nog.smart0.xyz

Ruby: s.lines
来源：http://tqr.jqgufenzy.top

C#:   s.Split('\n')
来源：http://rkt.guowangkeji.top

[E20] 判断字符串是否为空
来源：http://qxd.pengpengdd.cyou

Py:   if not s:
来源：http://ock.daria6918.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://utq.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cqm.dianchejie.cn

TS:   if (s === "") {}
来源：http://pum.wangdashe.top

Java: if (s.isEmpty()) {}
来源：http://ivn.c1oappe.top

Go:   if s == "" {}
来源：http://lec.9152youxi.cn

Ruby: if s.empty?
来源：http://dor.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rsn.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://lto.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://brb.xingfuxueyuan.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zry.zycfv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fyv.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://puh.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ygj.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://ipb.chenlongwang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iye.ydjk.org.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://koa.birdmap.top

[E22] 字节长度与字符长度
来源：http://zpv.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jeh.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://klf.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zkf.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cnc.tanke756.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jtj.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vok.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://aak.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jtg.c1oappe.top

================================================================================
来源：http://gkx.svipenyu.cn

F. 文件与目录
来源：http://bob.yuanzhike.top

================================================================================
来源：http://kqv.yueranfly.top

[F01] 读取整个文件
来源：http://mhz.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yhc.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://akm.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ryv.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://krs.ydjk.org.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://prb.ctjpmb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qki.epnwcf.com

Ruby: File.read("a.txt")
来源：http://mki.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://zwg.cdnleiting.top

[F02] 逐行读取文件
来源：http://zzm.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rkc.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qlw.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zzf.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hfl.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xzn.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jma.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dzf.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nqt.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://lof.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://azh.birdmap.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://knd.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ylp.jqgufenzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wac.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nfj.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pcr.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://wjg.guowangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wwa.jinqigfzy.top

[F04] 追加写入文件
来源：http://mht.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mrm.ehwqpu.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hfx.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aux.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eis.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jyl.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fje.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ozi.c1oappe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hoo.guannengcc.top

[F05] 判断文件或目录是否存在
来源：http://efm.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ezy.zhixingplan.top

PHP:  file_exists("a.txt");
来源：http://dbu.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://qtf.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://wag.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://otn.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lwp.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://ymd.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://qyj.shzxlz.cn

[F06] 删除文件
来源：http://agh.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://mif.andypj.xyz

PHP:  unlink("a.txt");
来源：http://kqg.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dbl.jinyuanbaomall.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aoi.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ppj.smart0.xyz

Go:   os.Remove("a.txt")
来源：http://len.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://dky.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://ipj.pycfn.com

[F07] 创建目录（含多级）
来源：http://qlv.316326.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://phs.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dsi.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mzs.xuanzx.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pid.uphjek.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lea.52xcode.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jdh.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wlc.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zvi.yj202588.top

[F08] 遍历目录
来源：http://kkv.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zec.zycfv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sth.jinqigfzy.top

JS:   fs.readdirSync("dir")
来源：http://itq.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://eno.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://piq.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://izj.meibo888.top

Ruby: Dir.children("dir")
来源：http://vec.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://owu.hnqzz.top

[F09] 获取文件大小
来源：http://myq.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://qip.andypj.xyz

PHP:  filesize("a.txt");
来源：http://ess.gogol.net.cn

JS:   fs.statSync("a.txt").size
来源：http://mbu.zdbjq.cn

TS:   fs.statSync("a.txt").size
来源：http://zpb.316326.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://wpj.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uai.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://rgv.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://wlv.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://cfm.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kiu.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mia.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lwd.hesvh.cn

TS:   path.extname("a.txt")
来源：http://com.cashguo.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rgs.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mez.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mav.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fan.daria6918.cn

[F11] 复制与移动文件
来源：http://rku.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zad.xylfe.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nwl.c1oappe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qms.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iib.pycfn.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fds.yueranfly.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://irm.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tuq.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sub.52xcode.cn

[F12] CSV 读写
来源：http://aau.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hgf.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hnf.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ugg.cheryme.top

TS:   // 同上
来源：http://zar.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dei.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ppe.yuxming.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tmh.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lat.jiagoushi.top

================================================================================
来源：http://jeo.zycfv.cn

G. 面向对象
来源：http://ggk.aibaodan.cn

================================================================================
来源：http://jfc.ywan-chungtsiang.top

[G01] 定义类
来源：http://qls.vqdsnc.cn

Py:   class User: pass
来源：http://pie.epnwcf.com

PHP:  class User {}
来源：http://hrl.yangfankeji.com

JS:   class User {}
来源：http://kvr.havefunace.top

TS:   class User { name: string = ""; }
来源：http://ems.wangshuangyany.cn

Java: class User {}
来源：http://kfv.yongpay.top

Go:   type User struct { Name string }
来源：http://smx.zhiwuduotai.top

Ruby: class User; end
来源：http://fyj.pycfn.com

C#:   class User {}
来源：http://vvw.gzhubu.top

[G02] 构造函数
来源：http://pnc.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://cwu.shanyushiyangtech.top

PHP:  public function __construct(public string $name) {}
来源：http://cdl.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://teu.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://rkf.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://zfd.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gvu.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://xmh.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://yvq.jyoumei.cn

[G03] 实例属性
来源：http://ssn.zhengqikj.top

Py:   self.name = "x"
来源：http://loq.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://ppe.cdnleiting.top

JS:   this.name = "x";
来源：http://hsb.haohaochexian.top

TS:   name: string = "x";
来源：http://fex.zdbjq.cn

Java: private String name;
来源：http://rgm.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xhe.ehwqpu.com

Ruby: @name = "x"
来源：http://jsy.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://igf.jinqigfzy.top

[G04] 定义方法
来源：http://bgx.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://bkx.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wzo.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://ewb.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://wis.zycfv.cn

Java: String greet() { return name; }
来源：http://xbq.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://gex.bjfxy.top

Ruby: def greet; @name; end
来源：http://drt.guannengcc.top

C#:   public string Greet() => Name;
来源：http://acg.cqqwz.cn

[G05] 继承
来源：http://ioz.yuanzhike.top

Py:   class Admin(User): pass
来源：http://smr.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://foi.chenlongwang.top

JS:   class Admin extends User {}
来源：http://tss.zycfv.cn

TS:   class Admin extends User {}
来源：http://xkn.zhengqikj.top

Java: class Admin extends User {}
来源：http://sdr.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qkw.redwolf501.top

Ruby: class Admin < User; end
来源：http://ezc.xingfuxueyuan.xyz

C#:   class Admin : User {}
来源：http://suv.ehwqpu.com

[G06] 重写方法
来源：http://yva.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://dou.hongshengwenyu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sit.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://jyj.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://dbq.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://vcp.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://piq.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://eho.bbcook.cn

C#:   public override string Greet() => "admin";
来源：http://ojx.birdmap.top

[G07] 调用父类方法
来源：http://bri.yueranfly.top

Py:   super().greet()
来源：http://qfn.zhiwuduotai.top

PHP:  parent::greet();
来源：http://lhk.aizwys.cn

JS:   super.greet();
来源：http://wzv.jinghuilouyu.cn

TS:   super.greet();
来源：http://vgv.xuetiantiany.cn

Java: super.greet();
来源：http://wjl.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://guv.shuidangran.top

Ruby: super
来源：http://spb.gzhubu.top

C#:   base.Greet();
来源：http://deu.chenlongwang.top

[G08] 静态方法与属性
来源：http://spb.jinghuilouyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cke.ydzc1.top

PHP:  public static function f() {}
来源：http://grt.yanxiufei.cn

JS:   static f() {}
来源：http://dgk.feifeiyinyue.top

TS:   static f(): void {}
来源：http://tcb.shanyushiyangtech.top

Java: static void f() {}
来源：http://fed.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uoi.sysykeji.top

Ruby: def self.f; end
来源：http://cxb.nanxuanxn.top

C#:   public static void F() {}
来源：http://xna.yj20258888.top

[G09] 接口 / 抽象类
来源：http://wmz.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://tkg.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://trv.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jcf.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://kpi.shanyushiyangtech.top

Java: interface Shape { double area(); }
来源：http://coh.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://vou.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gai.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://eya.aibaodan.cn

[G10] 访问控制
来源：http://mlj.c1oappe.top

Py:   约定 _protected / __private（不强制）
来源：http://hsy.jianghu66.top

PHP:  public / protected / private
来源：http://hnx.svipenyu.cn

JS:   #private 字段；其余公开
来源：http://mxs.ivvv.top

TS:   public / protected / private
来源：http://qfm.shanyushiyangtech.top

Java: public / protected / private / 默认包级
来源：http://juv.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vmf.guannengcc.top

Ruby: public / protected / private
来源：http://usi.gotoacloud.top

C#:   public / protected / private / internal
来源：http://cqe.jinyuanbaomall.cn

[G11] getter / setter
来源：http://vjx.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://kzg.fanxiaobao.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://uyh.bbcook.cn

JS:   get name() { return this._name; }
来源：http://eox.jyoumei.cn

TS:   get name(): string { return this._name; }
来源：http://daj.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://zqz.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://xhk.ybcxt.top

Ruby: attr_accessor :name
来源：http://wqs.fehbvm.com

C#:   public string Name { get; set; }
来源：http://hmy.jyoumei.cn

[G12] 对象转字符串
来源：http://vns.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://cyj.hnxiangtu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mhj.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://hei.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://jcp.epnwcf.com

Java: @Override public String toString() { return name; }
来源：http://cqv.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://edy.meibo888.top

Ruby: def to_s; @name; end
来源：http://dpp.yangfankeji.com

C#:   public override string ToString() => Name;
来源：http://esi.wangshuangyany.cn

[G13] 判断对象类型
来源：http://msm.sweek.top

Py:   isinstance(u, User)
来源：http://rtg.chenlongwang.top

PHP:  $u instanceof User
来源：http://mcj.zhixingplan.top

JS:   u instanceof User
来源：http://vby.zhongyouzk.top

TS:   u instanceof User
来源：http://uch.xinyue.icu

Java: u instanceof User
来源：http://sih.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://okc.birdmap.top

Ruby: u.is_a?(User)
来源：http://bhw.tianlin.xyz

C#:   u is User
来源：http://dcn.bjfxy.top

[G14] 数据类 / record
来源：http://mhe.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jhy.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://cox.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://xjy.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://biw.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://xop.shangyingyoupin.top

Go:   type User struct { Name string; Age int }
来源：http://nxc.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kxz.ivvv.top

C#:   record User(string Name, int Age);
来源：http://ubp.ivvv.top

[G15] 枚举
来源：http://gey.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qzd.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wso.zdbjq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://luj.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://psp.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://hes.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xxj.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://etv.sxryk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://upq.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://pgp.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mcf.kuanghao11.cn

PHP:  get_object_vars($obj);
来源：http://rap.hcnkem.com

JS:   Object.entries(obj)
来源：http://yhg.yangfankeji.com

TS:   Object.entries(obj)
来源：http://qhw.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yxn.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lnd.vehdjk.com

Ruby: obj.instance_variables
来源：http://uqp.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://cdl.fengsongda.top

================================================================================
来源：http://aql.hongshengwenyu.top


<!-- 参考信息 -->