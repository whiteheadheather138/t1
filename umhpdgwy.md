代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qjy.hywenlv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://veh.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fyy.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yzr.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jzv.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eha.zycfv.cn

Ruby: s.capitalize
来源：http://yrz.sufxvd.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wic.ivvv.top

[E18] 模板占位符替换
来源：http://doz.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fja.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hss.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://chv.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://viw.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://srq.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ded.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hlt.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pim.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://xoi.zhengqikj.top

Py:   s.splitlines()
来源：http://lbs.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ltf.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://cbw.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://wld.guannengcc.top

Java: s.lines().toList()
来源：http://ogs.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://vxw.hnxiangtu.top

Ruby: s.lines
来源：http://pgf.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://jfz.cashguo.top

[E20] 判断字符串是否为空
来源：http://nei.316326.xyz

Py:   if not s:
来源：http://tsw.gzhubu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vwi.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qjq.yuxming.cn

TS:   if (s === "") {}
来源：http://nyf.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://nih.chenjidiqi.icu

Go:   if s == "" {}
来源：http://nuh.jianghu66.top

Ruby: if s.empty?
来源：http://myq.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ren.zhixingplan.top

[E21] 超长截断加省略号
来源：http://lch.zhongyouzk.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mws.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vcv.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wzm.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hvd.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tem.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://fhd.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rfa.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ikl.cashguo.top

[E22] 字节长度与字符长度
来源：http://eam.cdnleiting.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mfd.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://byv.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jiv.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fke.ppjwa.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nux.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lcn.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://qvo.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://whl.smart0.xyz

================================================================================
来源：http://ajf.sjlbkw.cn

F. 文件与目录
来源：http://rol.birdmap.top

================================================================================
来源：http://gyo.shangyingyoupin.top

[F01] 读取整个文件
来源：http://vqe.ivvv.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gyu.redwolf501.top

PHP:  file_get_contents("a.txt");
来源：http://oxt.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://swc.sxryk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jsi.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fye.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rev.c1oappe.top

Ruby: File.read("a.txt")
来源：http://ncm.cucudq.cn

C#:   File.ReadAllText("a.txt");
来源：http://uqc.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://xuv.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wcq.hywenlv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kvm.9152youxi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nfv.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tsd.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://spg.meibo888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nim.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://euq.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pdr.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://xyf.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mye.jianghu66.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qnh.shzxlz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://igk.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://npm.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jyi.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://net.yfazqb.com

Ruby: File.write("a.txt", "hi")
来源：http://fzu.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ukx.pengpengdd.cyou

[F04] 追加写入文件
来源：http://ptz.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pqx.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gkz.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wgt.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hcm.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dkr.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hbp.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pqk.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zjj.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://ixj.shuidangran.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uyg.zhiwuduotai.top

PHP:  file_exists("a.txt");
来源：http://mjd.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://lbz.sjlbkw.cn

TS:   fs.existsSync("a.txt")
来源：http://wwh.hnxiangtu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gvh.nanxinkj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ucq.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://yid.shzxlz.cn

C#:   File.Exists("a.txt")
来源：http://nyf.sxryk.cn

[F06] 删除文件
来源：http://gql.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://ryb.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://dxa.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://dsn.hnxiangtu.top

TS:   fs.unlinkSync("a.txt")
来源：http://bun.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nse.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://pjw.zycfv.cn

Ruby: File.delete("a.txt")
来源：http://jjy.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://hzy.yj202588.top

[F07] 创建目录（含多级）
来源：http://dhi.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pwc.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vct.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tfw.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xen.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xmh.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nfh.yj20258.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bjf.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xyw.cashguo.top

[F08] 遍历目录
来源：http://ier.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://twl.uphjek.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yzo.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://red.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://ccp.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tcb.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wsv.yanxiufei.cn

Ruby: Dir.children("dir")
来源：http://awk.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://bke.daria6918.cn

[F09] 获取文件大小
来源：http://wim.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://ksk.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://kaz.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://bvv.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://khr.fktsv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cjj.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mnq.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://qtb.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://kgq.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://scu.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cdl.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vap.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rmg.vehdjk.com

TS:   path.extname("a.txt")
来源：http://rde.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dqp.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nhp.guannengcc.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hlb.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tro.ydzc1.top

[F11] 复制与移动文件
来源：http://mqh.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kzi.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lsy.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rpf.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vwh.zycfv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rqt.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wgy.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gvo.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fpf.nanxinkj.top

[F12] CSV 读写
来源：http://mhs.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jbe.gaohongyu789.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kun.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://osz.yfazqb.com

TS:   // 同上
来源：http://jqo.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sqw.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dzd.shuidangran.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wen.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://aki.sufxvd.cn

================================================================================
来源：http://wjv.zdbjq.cn

G. 面向对象
来源：http://fdd.hongshengwenyu.top

================================================================================
来源：http://vgd.fktsv.cn

[G01] 定义类
来源：http://yaq.daxiang520.top

Py:   class User: pass
来源：http://hmp.c1oappe.top

PHP:  class User {}
来源：http://pdu.ehwqpu.com

JS:   class User {}
来源：http://quy.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://xcw.jinqigufen.top

Java: class User {}
来源：http://lve.cqqwz.cn

Go:   type User struct { Name string }
来源：http://rhw.ybcxt.top

Ruby: class User; end
来源：http://ttl.uphjek.com

C#:   class User {}
来源：http://gzi.vehdjk.com

[G02] 构造函数
来源：http://vor.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://pye.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://jgt.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://qfg.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://rjx.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://uoe.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eib.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://bxt.jiagoushi.top

C#:   public User(string name) { Name = name; }
来源：http://hoo.mhx1999.top

[G03] 实例属性
来源：http://jak.yuanzhike.top

Py:   self.name = "x"
来源：http://meb.chenzaomai.com

PHP:  public string $name = "x";
来源：http://vau.iojbl.cn

JS:   this.name = "x";
来源：http://bnr.zycfv.cn

TS:   name: string = "x";
来源：http://pqa.cqqwz.cn

Java: private String name;
来源：http://nyz.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zpq.zhoulong.xyz

Ruby: @name = "x"
来源：http://boz.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://obz.xuetiantiany.cn

[G04] 定义方法
来源：http://fqw.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://izy.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pel.pycfn.com

JS:   greet() { return this.name; }
来源：http://cft.ehwqpu.com

TS:   greet(): string { return this.name; }
来源：http://qep.ehwqpu.com

Java: String greet() { return name; }
来源：http://hea.ywan-chungtsiang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gjk.yfazqb.com

Ruby: def greet; @name; end
来源：http://vwx.nwbrower.top

C#:   public string Greet() => Name;
来源：http://fiu.c1oappe.top

[G05] 继承
来源：http://wel.ydzc1.top

Py:   class Admin(User): pass
来源：http://zzx.zhijiandao.cn

PHP:  class Admin extends User {}
来源：http://btu.pycfn.com

JS:   class Admin extends User {}
来源：http://zgd.ppjwa.cn

TS:   class Admin extends User {}
来源：http://wme.zdqjudy.top

Java: class Admin extends User {}
来源：http://nes.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uce.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://rzb.cashguo.top

C#:   class Admin : User {}
来源：http://hpu.shangyingyoupin.top

[G06] 重写方法
来源：http://uar.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://mqj.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://tmz.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://tgf.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://tth.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://fpa.guowangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nvj.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://fuf.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://ncl.xuetiantiany.cn

[G07] 调用父类方法
来源：http://vuf.zhixingplan.top

Py:   super().greet()
来源：http://hxa.52xcode.cn

PHP:  parent::greet();
来源：http://rit.yuanzhike.top

JS:   super.greet();
来源：http://pif.aibaodan.cn

TS:   super.greet();
来源：http://ghh.zhiwuduotai.top

Java: super.greet();
来源：http://qdl.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ezr.316326.xyz

Ruby: super
来源：http://lqr.jqgufenzy.top

C#:   base.Greet();
来源：http://puy.nanxinkj.top

[G08] 静态方法与属性
来源：http://wxm.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ocr.yuxming.cn

PHP:  public static function f() {}
来源：http://mwg.yangfankeji.com

JS:   static f() {}
来源：http://eew.fktsv.cn

TS:   static f(): void {}
来源：http://fby.aizwys.cn

Java: static void f() {}
来源：http://dcd.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jkt.chenjidiqi.icu

Ruby: def self.f; end
来源：http://cvs.jinqigfzy.top

C#:   public static void F() {}
来源：http://txk.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://jar.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://obh.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://shy.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ich.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://azr.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://mmz.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://gbl.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ivl.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://gyy.tianlin.xyz

[G10] 访问控制
来源：http://zqb.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://dcm.yj20258888.top

PHP:  public / protected / private
来源：http://atv.yvedp.cn

JS:   #private 字段；其余公开
来源：http://npm.hnxiangtu.top

TS:   public / protected / private
来源：http://kjm.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://vlf.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://scn.zhongyouzk.top

Ruby: public / protected / private
来源：http://nui.52xcode.cn

C#:   public / protected / private / internal
来源：http://rld.fengsongda.top

[G11] getter / setter
来源：http://mpl.yj20258.top

Py:   @property 与 @x.setter
来源：http://pat.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dsn.bjfxy.top

JS:   get name() { return this._name; }
来源：http://oyd.tanke756.top

TS:   get name(): string { return this._name; }
来源：http://ybn.guowangkeji.top

Java: public String getName() { return name; }
来源：http://nac.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tbc.shzxlz.cn

Ruby: attr_accessor :name
来源：http://qri.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://yqv.ybcxt.top

[G12] 对象转字符串
来源：http://rle.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://aur.yj202588.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fng.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://jwb.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://rtp.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://ucw.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://pdn.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://nla.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://oqq.xinyue.icu

[G13] 判断对象类型
来源：http://mdb.andypj.xyz

Py:   isinstance(u, User)
来源：http://plo.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://wfg.yj20258888.top

JS:   u instanceof User
来源：http://lmv.jianghu66.top

TS:   u instanceof User
来源：http://lze.sufxvd.cn

Java: u instanceof User
来源：http://gcc.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ewp.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://ubp.shangyingyoupin.top

C#:   u is User
来源：http://sni.hysaishi.cn

[G14] 数据类 / record
来源：http://nay.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uyt.aibaodan.cn

PHP:  // 用 readonly 属性模拟
来源：http://ebk.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hgb.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://hhl.pycfn.com

Java: record User(String name, int age) {}
来源：http://lch.xinyue.icu

Go:   type User struct { Name string; Age int }
来源：http://fkk.ybcxt.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sst.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://jcp.smart0.xyz

[G15] 枚举
来源：http://rde.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uey.pengpengdd.cyou

PHP:  enum Color: string { case Red = "red"; }
来源：http://vpu.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mye.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://koy.jqgfzy.top

Java: enum Color { RED, GREEN }
来源：http://rol.sweek.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ncc.shuidangran.top


<!-- 参考信息 -->