代发 wailian999

PHP:  number_format(1234567);
来源：http://vjp.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://jme.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://gpo.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cfk.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rog.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lbq.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://sxk.daria6918.cn

[E17] 首字母大写
来源：http://cgc.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fpc.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ota.jyoumei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gww.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wcg.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wts.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sqf.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://lla.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://utf.ctjpmb.com

[E18] 模板占位符替换
来源：http://oca.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mwv.dashuyun.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fxp.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hcm.zdqjudy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zie.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vhg.nanxuanxn.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://soe.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://app.0kj1m.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qoy.ydzc1.top

[E19] 多行文本按行拆分
来源：http://piu.andypj.xyz

Py:   s.splitlines()
来源：http://iok.zhaomingkeji.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dcq.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://imc.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://tko.yueranfly.top

Java: s.lines().toList()
来源：http://hxg.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://fvv.xuanzx.com

Ruby: s.lines
来源：http://bps.hfpthk.cn

C#:   s.Split('\n')
来源：http://nee.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://iis.zhijiandao.cn

Py:   if not s:
来源：http://tlw.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://esp.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hcx.yuanzhike.top

TS:   if (s === "") {}
来源：http://uhb.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://mdv.vehdjk.com

Go:   if s == "" {}
来源：http://qbo.fzhhl.top

Ruby: if s.empty?
来源：http://onh.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://abe.shuidangran.top

[E21] 超长截断加省略号
来源：http://gkj.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jsl.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ngy.fehbvm.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yxu.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yft.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zwp.fzhhl.top

Go:   // 按 rune 判断长度后截断
来源：http://zqz.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://noi.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ncx.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://pyj.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pui.hammf.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dje.yuxming.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ubq.bjfxy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hpx.tanke756.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://caz.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cif.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://wre.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ssk.pycfn.com

================================================================================
来源：http://ysp.andypj.xyz

F. 文件与目录
来源：http://yft.yfazqb.com

================================================================================
来源：http://pzb.chenjidiqi.icu

[F01] 读取整个文件
来源：http://nbv.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hrx.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://ovs.sjlbkw.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ozc.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dlt.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://mkx.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vdl.daria6918.cn

Ruby: File.read("a.txt")
来源：http://pbc.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://qje.aizwys.cn

[F02] 逐行读取文件
来源：http://mym.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fvw.hywenlv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://imo.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tig.cdnleiting.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sbf.yuxming.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ogy.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qzq.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mol.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://flc.birdmap.top

[F03] 写入文件（覆盖）
来源：http://tbx.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nnt.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://nlf.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mqs.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hbd.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ydd.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://inv.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://knv.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eck.nwbrower.top

[F04] 追加写入文件
来源：http://gmi.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dvc.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nbi.ehwqpu.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gny.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ttr.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vec.zycfv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bhh.andypj.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qac.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qas.hammf.cn

[F05] 判断文件或目录是否存在
来源：http://gzv.yonumen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dub.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://pjd.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://xeb.zhengqikj.top

TS:   fs.existsSync("a.txt")
来源：http://hvf.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vsv.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vzf.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://gyp.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://smx.havefunace.top

[F06] 删除文件
来源：http://meo.jinyuanbaomall.cn

Py:   os.remove("a.txt")
来源：http://jur.chenzaomai.com

PHP:  unlink("a.txt");
来源：http://bus.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://msm.kuanghao11.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sfo.uphjek.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://obp.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://ygp.fzhhl.top

Ruby: File.delete("a.txt")
来源：http://nzk.xingfuxueyuan.xyz

C#:   File.Delete("a.txt");
来源：http://unv.gogol.net.cn

[F07] 创建目录（含多级）
来源：http://bsp.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jwe.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kch.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baw.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://afo.birdmap.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rfz.yongpay.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://umc.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iiw.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hnk.hysaishi.cn

[F08] 遍历目录
来源：http://jos.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mce.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sfz.daxiang520.top

JS:   fs.readdirSync("dir")
来源：http://utn.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://jvr.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://grh.hnqzz.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bta.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://uzz.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://ibw.hcnkem.com

[F09] 获取文件大小
来源：http://isl.ydzc1.top

Py:   os.path.getsize("a.txt")
来源：http://icj.tanke756.top

PHP:  filesize("a.txt");
来源：http://hpn.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://xcj.jiagoushi.top

TS:   fs.statSync("a.txt").size
来源：http://aan.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://czk.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mos.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://nsw.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://noc.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://vvv.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ddn.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://adu.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bbt.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://uyr.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://csy.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cjj.gzhubu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nrb.nanxinkj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yjg.tianlin.xyz

[F11] 复制与移动文件
来源：http://bqw.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fex.hysaishi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xnt.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mal.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://buv.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lnz.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yrj.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ges.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rnx.redwolf501.top

[F12] CSV 读写
来源：http://ape.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qhd.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fke.daxiang520.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cqp.shangyingyoupin.top

TS:   // 同上
来源：http://ffg.yj20258.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jjm.tanke756.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wgn.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://thz.tarul.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://leb.smart0.xyz

================================================================================
来源：http://ehq.tianlin.xyz

G. 面向对象
来源：http://mvr.dianchejie.cn

================================================================================
来源：http://dnt.jlsjyb.cn

[G01] 定义类
来源：http://ziw.c1oappe.top

Py:   class User: pass
来源：http://hlx.gzhubu.top

PHP:  class User {}
来源：http://dmc.yangfankeji.com

JS:   class User {}
来源：http://gyw.cashguo.top

TS:   class User { name: string = ""; }
来源：http://ebf.vehdjk.com

Java: class User {}
来源：http://qhm.shuidangran.top

Go:   type User struct { Name string }
来源：http://dim.c1oappe.top

Ruby: class User; end
来源：http://eyp.0kj1m.cn

C#:   class User {}
来源：http://cxh.iojbl.cn

[G02] 构造函数
来源：http://sct.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://euu.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://txi.hywenlv.cn

JS:   constructor(name) { this.name = name; }
来源：http://euw.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://cvl.ydjk.org.cn

Java: User(String name) { this.name = name; }
来源：http://dex.hesvh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sqf.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://nan.316326.xyz

C#:   public User(string name) { Name = name; }
来源：http://ogz.xylfe.cn

[G03] 实例属性
来源：http://tzp.sxryk.cn

Py:   self.name = "x"
来源：http://elh.xuanzx.com

PHP:  public string $name = "x";
来源：http://ckf.vqdsnc.cn

JS:   this.name = "x";
来源：http://utw.dashuyun.cn

TS:   name: string = "x";
来源：http://ryc.snrcjt.cn

Java: private String name;
来源：http://gme.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ewj.jinqigufen.top

Ruby: @name = "x"
来源：http://kdg.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://cqt.sufxvd.cn

[G04] 定义方法
来源：http://hjk.uphjek.com

Py:   def greet(self): return self.name
来源：http://kld.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://aru.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://rro.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://get.yangfankeji.com

Java: String greet() { return name; }
来源：http://qpa.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tsx.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://jcq.epnwcf.com

C#:   public string Greet() => Name;
来源：http://xvk.yuanzhike.top

[G05] 继承
来源：http://bik.zdqjudy.top

Py:   class Admin(User): pass
来源：http://czw.zhaomingkeji.xyz

PHP:  class Admin extends User {}
来源：http://bvk.sweek.top

JS:   class Admin extends User {}
来源：http://fkv.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://bdf.dashuyun.cn

Java: class Admin extends User {}
来源：http://qnk.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://olw.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://uzf.nanxuanxn.top

C#:   class Admin : User {}
来源：http://dfl.jiagoushi.top

[G06] 重写方法
来源：http://lhu.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://qav.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ewv.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://rue.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://zwv.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://jab.xylfe.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nve.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://zrb.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://vmt.gotoacloud.top

[G07] 调用父类方法
来源：http://ejn.quarkkingdee.top

Py:   super().greet()
来源：http://rck.zhengqikj.top

PHP:  parent::greet();
来源：http://foj.sufxvd.cn

JS:   super.greet();
来源：http://gfw.jyoumei.cn

TS:   super.greet();
来源：http://fvj.sjlbkw.cn

Java: super.greet();
来源：http://vxa.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xdc.zhiwuduotai.top

Ruby: super
来源：http://enx.shanyushiyangkeji.top

C#:   base.Greet();
来源：http://tvm.iojbl.cn

[G08] 静态方法与属性
来源：http://awo.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uop.cashguo.top

PHP:  public static function f() {}
来源：http://czq.jlsjyb.cn

JS:   static f() {}
来源：http://faw.tanke756.top

TS:   static f(): void {}
来源：http://fio.yj20258888.top

Java: static void f() {}
来源：http://tri.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uav.fktsv.cn

Ruby: def self.f; end
来源：http://dem.jiagoushi.top

C#:   public static void F() {}
来源：http://fbc.bbcook.cn

[G09] 接口 / 抽象类
来源：http://scc.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://auk.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://dlw.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hzz.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://aqa.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://exn.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://nqj.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nwf.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://zsy.hnqzz.top

[G10] 访问控制
来源：http://vii.yangfankeji.com

Py:   约定 _protected / __private（不强制）
来源：http://btg.tanke756.top

PHP:  public / protected / private
来源：http://qiw.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://awg.fehbvm.com

TS:   public / protected / private
来源：http://hyd.dianchejie.cn

Java: public / protected / private / 默认包级
来源：http://xik.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bro.guowangkeji.top

Ruby: public / protected / private
来源：http://buo.shzxlz.cn

C#:   public / protected / private / internal
来源：http://fvf.bjfxy.top

[G11] getter / setter
来源：http://jqu.tian-w.cn

Py:   @property 与 @x.setter
来源：http://vwk.hfpthk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zoy.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://jfz.sysykeji.top

TS:   get name(): string { return this._name; }
来源：http://rhh.yj20258888.top

Java: public String getName() { return name; }
来源：http://hbu.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gcx.xylfe.cn

Ruby: attr_accessor :name
来源：http://btg.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://vtb.ctjpmb.com

[G12] 对象转字符串
来源：http://jgq.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://suo.0kj1m.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wvt.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://xtd.ydzc1.top

TS:   toString(): string { return this.name; }
来源：http://agd.kuanghao11.cn

Java: @Override public String toString() { return name; }
来源：http://vdj.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://hkg.sweek.top

Ruby: def to_s; @name; end
来源：http://vki.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://xab.smart0.xyz

[G13] 判断对象类型
来源：http://uvj.bbcook.cn

Py:   isinstance(u, User)
来源：http://arq.hysaishi.cn

PHP:  $u instanceof User
来源：http://npk.shanyushiyangtech.top

JS:   u instanceof User
来源：http://dpq.fktsv.cn

TS:   u instanceof User
来源：http://sbc.ivvv.top

Java: u instanceof User
来源：http://pmu.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cww.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://woc.tianlin.xyz

C#:   u is User
来源：http://bgr.tianlin.xyz

[G14] 数据类 / record
来源：http://lik.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vsp.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://nca.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://xdb.ydjk.org.cn

TS:   type User = { name: string; age: number };
来源：http://miu.sweek.top

Java: record User(String name, int age) {}
来源：http://lvz.feifeiyinyue.top

Go:   type User struct { Name string; Age int }
来源：http://viz.yj202588.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://skd.iojbl.cn


<!-- 参考信息 -->