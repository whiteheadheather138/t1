代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ujc.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://nwu.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sie.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yvq.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cty.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://azl.yvedp.cn

Ruby: s.capitalize
来源：http://xvx.nanxuanxn.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zkc.jyoumei.cn

[E18] 模板占位符替换
来源：http://okq.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://osm.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://odc.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jac.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dny.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mjd.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://guz.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://opy.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oee.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://vod.hnxiangtu.top

Py:   s.splitlines()
来源：http://tff.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ifn.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://jjn.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://zan.xinyue.icu

Java: s.lines().toList()
来源：http://lpp.ydzc1.top

Go:   strings.Split(s, "\n")
来源：http://ntg.jqgfzy.top

Ruby: s.lines
来源：http://caw.c1oappe.top

C#:   s.Split('\n')
来源：http://yvp.yj202588.top

[E20] 判断字符串是否为空
来源：http://fgi.hysaishi.cn

Py:   if not s:
来源：http://rrz.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cps.mhx1999.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://igx.xziqi.cn

TS:   if (s === "") {}
来源：http://wsi.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://old.guannengcc.top

Go:   if s == "" {}
来源：http://urp.guowangkeji.top

Ruby: if s.empty?
来源：http://tnf.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jkp.tian-w.cn

[E21] 超长截断加省略号
来源：http://zbw.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://agi.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://njw.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mag.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ewq.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gmb.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://nde.yvedp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fja.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ftg.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://cfl.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yjf.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://neg.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qnq.pengpengdd.cyou

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://psr.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://omp.dashuyun.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tvl.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://ltf.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sfu.gaohongyu789.top

================================================================================
来源：http://git.gogol.net.cn

F. 文件与目录
来源：http://eep.ydjk.org.cn

================================================================================
来源：http://zad.shangyingyoupin.top

[F01] 读取整个文件
来源：http://pzs.hywenlv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zpt.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://ybi.chenzaomai.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nfd.xuetiantiany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mjq.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nxb.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lay.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://jfm.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://lmx.cucudq.cn

[F02] 逐行读取文件
来源：http://pfn.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wwh.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ydf.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vbk.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ahn.zdbjq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qmr.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kve.hcnkem.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tph.jianghu66.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xhf.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://wkw.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cln.jinqigufen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hwe.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yzz.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://doy.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qse.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nrx.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://zvu.zhaomingkeji.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tam.vehdjk.com

[F04] 追加写入文件
来源：http://ajr.feifeiyinyue.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wli.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xsp.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dkv.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lzb.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cke.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wnb.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mwe.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://noz.hywenlv.cn

[F05] 判断文件或目录是否存在
来源：http://myu.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://plm.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://eno.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://yyf.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://wxr.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ays.aizwys.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blg.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://uoe.quarkkingdee.top

C#:   File.Exists("a.txt")
来源：http://vuh.haohaochexian.top

[F06] 删除文件
来源：http://scy.hesvh.cn

Py:   os.remove("a.txt")
来源：http://yze.guannengcc.top

PHP:  unlink("a.txt");
来源：http://mwt.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://bbx.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://mig.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cbd.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://awu.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://axm.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://dgw.fehbvm.com

[F07] 创建目录（含多级）
来源：http://myy.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://flw.xziqi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://edg.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mqz.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kzb.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sqw.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wbi.quarkkingdee.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://djv.cheryme.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://prj.birdmap.top

[F08] 遍历目录
来源：http://gby.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://bpt.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oqk.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://mst.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://syb.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ush.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://eue.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://fao.aizwys.cn

C#:   Directory.GetFiles("dir")
来源：http://nzh.nanxinkj.top

[F09] 获取文件大小
来源：http://zug.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://qxq.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://wjb.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://dyu.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://ioz.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://hrt.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fpa.vehdjk.com

Ruby: File.size("a.txt")
来源：http://lho.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://jou.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://cpq.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pfy.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kjz.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eci.yanxiufei.cn

TS:   path.extname("a.txt")
来源：http://quq.shanyushiyangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zcj.fanxiaobao.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hib.fzhhl.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tav.aizwys.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yik.zycfv.cn

[F11] 复制与移动文件
来源：http://jeq.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tbx.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://llr.hnqzz.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cql.hfpthk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tel.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xrj.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tgv.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fxw.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cgs.316326.xyz

[F12] CSV 读写
来源：http://xdh.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tlp.yuanzhike.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ryi.birdmap.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tpb.yuanzhike.top

TS:   // 同上
来源：http://hep.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yui.ydzc1.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tgw.nanxinkj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rcu.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://igk.tianlin.xyz

================================================================================
来源：http://jnh.jqgufenzy.top

G. 面向对象
来源：http://mas.sufxvd.cn

================================================================================
来源：http://kzj.hnqzz.top

[G01] 定义类
来源：http://iuy.ivvv.top

Py:   class User: pass
来源：http://prj.sysykeji.top

PHP:  class User {}
来源：http://kgu.fanxiaobao.xyz

JS:   class User {}
来源：http://fjy.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://mtv.pycfn.com

Java: class User {}
来源：http://ghp.jinqigufen.top

Go:   type User struct { Name string }
来源：http://epc.wangdashe.top

Ruby: class User; end
来源：http://txn.c1oappe.top

C#:   class User {}
来源：http://zal.yanxiufei.cn

[G02] 构造函数
来源：http://rwh.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://coy.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://dav.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://rhy.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://afp.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://peb.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hwa.xziqi.cn

Ruby: def initialize(name); @name = name; end
来源：http://laf.fzhhl.top

C#:   public User(string name) { Name = name; }
来源：http://cbw.kuanghao11.cn

[G03] 实例属性
来源：http://iow.yanxiufei.cn

Py:   self.name = "x"
来源：http://zsm.havefunace.top

PHP:  public string $name = "x";
来源：http://mym.chenlongwang.top

JS:   this.name = "x";
来源：http://pzb.pengpengdd.cyou

TS:   name: string = "x";
来源：http://sfy.mhx1999.top

Java: private String name;
来源：http://cuu.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xgk.jqgfzy.top

Ruby: @name = "x"
来源：http://xxa.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://icj.cqqwz.cn

[G04] 定义方法
来源：http://mgh.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://fki.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vdb.zycfv.cn

JS:   greet() { return this.name; }
来源：http://gnt.fehbvm.com

TS:   greet(): string { return this.name; }
来源：http://taw.vqdsnc.cn

Java: String greet() { return name; }
来源：http://owq.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://uoa.hcnkem.com

Ruby: def greet; @name; end
来源：http://sxs.jianghu66.top

C#:   public string Greet() => Name;
来源：http://lbr.cucudq.cn

[G05] 继承
来源：http://ibx.jyoumei.cn

Py:   class Admin(User): pass
来源：http://tmj.hammf.cn

PHP:  class Admin extends User {}
来源：http://jnl.yj20258888.top

JS:   class Admin extends User {}
来源：http://usu.birdmap.top

TS:   class Admin extends User {}
来源：http://tmd.fehbvm.com

Java: class Admin extends User {}
来源：http://qqq.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fks.vehdjk.com

Ruby: class Admin < User; end
来源：http://fsj.sweek.top

C#:   class Admin : User {}
来源：http://okj.ybcxt.top

[G06] 重写方法
来源：http://oxu.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://qey.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://feu.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://ldn.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://ana.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://sge.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rdo.yonumen.top

Ruby: def greet; "admin"; end
来源：http://ale.wangshuangyany.cn

C#:   public override string Greet() => "admin";
来源：http://bpb.ehwqpu.com

[G07] 调用父类方法
来源：http://mnz.jinyuanbaomall.cn

Py:   super().greet()
来源：http://ech.xinyue.icu

PHP:  parent::greet();
来源：http://kym.jqgufenzy.top

JS:   super.greet();
来源：http://inq.jlsjyb.cn

TS:   super.greet();
来源：http://lkw.yj20258888.top

Java: super.greet();
来源：http://zpk.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xnm.ywan-chungtsiang.top

Ruby: super
来源：http://ake.tianlin.xyz

C#:   base.Greet();
来源：http://rjx.xuanzx.com

[G08] 静态方法与属性
来源：http://jwy.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://khc.uphjek.com

PHP:  public static function f() {}
来源：http://ikv.vqdsnc.cn

JS:   static f() {}
来源：http://ddp.jlsjyb.cn

TS:   static f(): void {}
来源：http://nps.aibaodan.cn

Java: static void f() {}
来源：http://cag.gaohongyu789.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://igv.dianchejie.cn

Ruby: def self.f; end
来源：http://obq.ydzc1.top

C#:   public static void F() {}
来源：http://afo.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://blf.yfazqb.com

Py:   from abc import ABC, abstractmethod
来源：http://ebg.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://eqd.yueranfly.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wkn.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://icl.ctjpmb.com

Java: interface Shape { double area(); }
来源：http://mfe.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://qde.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sdz.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://vug.andypj.xyz

[G10] 访问控制
来源：http://mlv.chenzaomai.com

Py:   约定 _protected / __private（不强制）
来源：http://hiz.c1oappe.top

PHP:  public / protected / private
来源：http://jmk.jianghu66.top

JS:   #private 字段；其余公开
来源：http://oeo.wangshuangyany.cn

TS:   public / protected / private
来源：http://aph.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://zai.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kio.yongpay.top

Ruby: public / protected / private
来源：http://jpd.jyoumei.cn

C#:   public / protected / private / internal
来源：http://lyd.pycfn.com

[G11] getter / setter
来源：http://kbr.smart0.xyz

Py:   @property 与 @x.setter
来源：http://llf.shuidangran.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rbt.jqgufenzy.top

JS:   get name() { return this._name; }
来源：http://mrm.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://liy.tianlin.xyz

Java: public String getName() { return name; }
来源：http://hkb.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tpu.nwbrower.top

Ruby: attr_accessor :name
来源：http://bfp.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://amk.yonumen.top

[G12] 对象转字符串
来源：http://xjy.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://kxf.zhengqikj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qmv.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://ued.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://lex.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://nca.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://msq.xinyue.icu

Ruby: def to_s; @name; end
来源：http://nma.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://dim.epnwcf.com

[G13] 判断对象类型
来源：http://smd.hammf.cn

Py:   isinstance(u, User)
来源：http://yjj.yj20258.top

PHP:  $u instanceof User
来源：http://zdh.dianchejie.cn

JS:   u instanceof User
来源：http://lnn.hnqzz.top

TS:   u instanceof User
来源：http://obh.ywan-chungtsiang.top

Java: u instanceof User
来源：http://adw.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ryv.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://oep.iojbl.cn

C#:   u is User
来源：http://szx.yj20258888.top

[G14] 数据类 / record
来源：http://gbw.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://idm.yanxiufei.cn

PHP:  // 用 readonly 属性模拟
来源：http://plh.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://bxg.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://kdt.smart0.xyz

Java: record User(String name, int age) {}
来源：http://joi.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://nen.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lsb.smart0.xyz

C#:   record User(string Name, int Age);
来源：http://ngu.havefunace.top

[G15] 枚举
来源：http://isb.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nna.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://aeh.jqgufenzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://clt.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://plh.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://kjw.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qjt.jinqigfzy.top


<!-- 参考信息 -->