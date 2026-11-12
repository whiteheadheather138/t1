代发 wailian999

PHP:  number_format(1234567);
来源：http://ybr.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://pom.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yyx.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://grm.daria6918.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qqd.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dsd.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://pdk.svipenyu.cn

[E17] 首字母大写
来源：http://grq.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xhj.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ils.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cqa.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lqv.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://amn.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dua.birdmap.top

Ruby: s.capitalize
来源：http://kwj.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ihj.hammf.cn

[E18] 模板占位符替换
来源：http://vzl.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gap.yfazqb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ohe.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://maf.aizwys.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iig.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xms.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rcg.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pzr.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zqe.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://ago.ydzc1.top

Py:   s.splitlines()
来源：http://uwp.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gno.ydzc1.top

JS:   s.split(/\r?\n/)
来源：http://cmq.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://dfp.jinqigfzy.top

Java: s.lines().toList()
来源：http://clm.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://fgc.cqqwz.cn

Ruby: s.lines
来源：http://pgw.quarkkingdee.top

C#:   s.Split('\n')
来源：http://wht.yuanzhike.top

[E20] 判断字符串是否为空
来源：http://zxx.xuetiantiany.cn

Py:   if not s:
来源：http://wex.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://axr.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bcq.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://jtq.gogol.net.cn

Java: if (s.isEmpty()) {}
来源：http://cyq.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://ayh.hnqzz.top

Ruby: if s.empty?
来源：http://zhh.chenzaomai.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nds.yvedp.cn

[E21] 超长截断加省略号
来源：http://csi.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fso.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rdb.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://alx.tanke756.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://brr.xylfe.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tux.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://frb.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ckv.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eyq.ehwqpu.com

[E22] 字节长度与字符长度
来源：http://vtf.haohaochexian.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zda.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kkg.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yvt.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fcp.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jkg.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gvj.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://iqf.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mdw.haohaochexian.top

================================================================================
来源：http://tcs.ehwqpu.com

F. 文件与目录
来源：http://ngj.xziqi.cn

================================================================================
来源：http://vte.xinyue.icu

[F01] 读取整个文件
来源：http://idc.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qzp.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://nmz.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zhv.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hof.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://scv.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rqc.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://yqz.shanyushiyangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://lid.hnqzz.top

[F02] 逐行读取文件
来源：http://blz.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://udx.sysykeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wai.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gsh.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pyi.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ain.gzhubu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ggd.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dyk.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dfp.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://njm.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zzk.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xmg.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ygt.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ize.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ivz.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mel.hnqzz.top

Ruby: File.write("a.txt", "hi")
来源：http://jku.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mdu.zycfv.cn

[F04] 追加写入文件
来源：http://vaj.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gvl.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nlc.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zqw.chenjidiqi.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ogw.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dyb.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://czy.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nix.quarkkingdee.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qaf.gzhubu.top

[F05] 判断文件或目录是否存在
来源：http://yha.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ykp.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://pbz.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://cwj.tian-w.cn

TS:   fs.existsSync("a.txt")
来源：http://neq.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eyi.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iol.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://ciz.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://fel.zhongyouzk.top

[F06] 删除文件
来源：http://kmv.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://zye.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://bjm.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://upa.epnwcf.com

TS:   fs.unlinkSync("a.txt")
来源：http://ojo.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pmk.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://vyf.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://xdg.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://lqx.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://abr.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bsk.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kky.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ejm.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aak.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zce.dashuyun.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uca.hfpthk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pfv.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mux.gogol.net.cn

[F08] 遍历目录
来源：http://ojq.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ear.uphjek.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jbu.bjfxy.top

JS:   fs.readdirSync("dir")
来源：http://cdy.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://vhw.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vqj.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uex.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://ldy.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://pio.cdnleiting.top

[F09] 获取文件大小
来源：http://tlg.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://hki.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://ybp.birdmap.top

JS:   fs.statSync("a.txt").size
来源：http://ffb.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://lym.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://bju.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pqk.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://gtp.gzhubu.top

C#:   new FileInfo("a.txt").Length
来源：http://wyo.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://rgn.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://etw.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pfr.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://naz.yanxiufei.cn

TS:   path.extname("a.txt")
来源：http://zlh.yongpay.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pcp.gzhubu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gbq.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tpk.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vur.zhengqikj.top

[F11] 复制与移动文件
来源：http://wxd.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yps.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://upo.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wke.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tep.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://atk.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kow.hfpthk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mip.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zoa.tarul.cn

[F12] CSV 读写
来源：http://jqj.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xah.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qgu.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ylr.jqgufenzy.top

TS:   // 同上
来源：http://oqg.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hud.cqqwz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nnp.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mki.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lia.gzhubu.top

================================================================================
来源：http://rpj.jinghuilouyu.cn

G. 面向对象
来源：http://wic.cdnleiting.top

================================================================================
来源：http://mfw.yuanzhike.top

[G01] 定义类
来源：http://kto.chenlongwang.top

Py:   class User: pass
来源：http://gye.yanxiufei.cn

PHP:  class User {}
来源：http://dys.nwbrower.top

JS:   class User {}
来源：http://qxr.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://yzo.wangdashe.top

Java: class User {}
来源：http://kin.fengsongda.top

Go:   type User struct { Name string }
来源：http://qrb.guannengcc.top

Ruby: class User; end
来源：http://ugr.gotoacloud.top

C#:   class User {}
来源：http://guo.316326.xyz

[G02] 构造函数
来源：http://ouu.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://xyl.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://ttn.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://zvs.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://fyr.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://rwh.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://leu.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://fwj.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://hdo.jinghuilouyu.cn

[G03] 实例属性
来源：http://mpt.svipenyu.cn

Py:   self.name = "x"
来源：http://wsk.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://gcd.ywan-chungtsiang.top

JS:   this.name = "x";
来源：http://urg.52xcode.cn

TS:   name: string = "x";
来源：http://ywv.redwolf501.top

Java: private String name;
来源：http://tps.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fmy.wangdashe.top

Ruby: @name = "x"
来源：http://lgg.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://hyw.smart0.xyz

[G04] 定义方法
来源：http://cse.hfpthk.cn

Py:   def greet(self): return self.name
来源：http://ejw.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cqv.ybcxt.top

JS:   greet() { return this.name; }
来源：http://xet.yuanzhike.top

TS:   greet(): string { return this.name; }
来源：http://krx.yangfankeji.com

Java: String greet() { return name; }
来源：http://bws.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ipk.wangdashe.top

Ruby: def greet; @name; end
来源：http://hkl.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://ihq.zhixingplan.top

[G05] 继承
来源：http://fml.meibo888.top

Py:   class Admin(User): pass
来源：http://amn.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://jfz.tanke756.top

JS:   class Admin extends User {}
来源：http://jaw.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://tge.tarul.cn

Java: class Admin extends User {}
来源：http://loz.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bub.nwbrower.top

Ruby: class Admin < User; end
来源：http://jss.birdmap.top

C#:   class Admin : User {}
来源：http://eah.shzxlz.cn

[G06] 重写方法
来源：http://gsf.shangyingyoupin.top

Py:   def greet(self): return "admin"
来源：http://psp.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aaj.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://vxp.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://tvd.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://ppq.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fjs.yonumen.top

Ruby: def greet; "admin"; end
来源：http://tkp.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://bms.guannengcc.top

[G07] 调用父类方法
来源：http://tuh.shanyushiyangkeji.top

Py:   super().greet()
来源：http://cws.gaohongyu789.top

PHP:  parent::greet();
来源：http://pfr.epnwcf.com

JS:   super.greet();
来源：http://gzh.zycfv.cn

TS:   super.greet();
来源：http://zaj.pengpengdd.cyou

Java: super.greet();
来源：http://uac.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yzt.fengsongda.top

Ruby: super
来源：http://wad.xziqi.cn

C#:   base.Greet();
来源：http://ezn.smart0.xyz

[G08] 静态方法与属性
来源：http://wpp.ppjwa.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gfx.aibaodan.cn

PHP:  public static function f() {}
来源：http://kzd.iojbl.cn

JS:   static f() {}
来源：http://dfj.fengsongda.top

TS:   static f(): void {}
来源：http://cxx.hysaishi.cn

Java: static void f() {}
来源：http://usv.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wwm.guowangkeji.top

Ruby: def self.f; end
来源：http://jzm.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://xes.tian-w.cn

[G09] 接口 / 抽象类
来源：http://jyp.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://oct.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ebt.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://xhz.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://tdz.jyoumei.cn

Java: interface Shape { double area(); }
来源：http://dcj.iojbl.cn

Go:   type Shape interface { Area() float64 }
来源：http://wpo.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ioj.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://xqm.xuanzx.com

[G10] 访问控制
来源：http://wud.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://nsb.dashuyun.cn

PHP:  public / protected / private
来源：http://rbg.ivvv.top

JS:   #private 字段；其余公开
来源：http://rdm.nanxuanxn.top

TS:   public / protected / private
来源：http://vnf.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://bgp.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vka.daria6918.cn

Ruby: public / protected / private
来源：http://rmd.52xcode.cn

C#:   public / protected / private / internal
来源：http://hha.yj20258888.top

[G11] getter / setter
来源：http://epn.yj202588.top

Py:   @property 与 @x.setter
来源：http://pzw.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qnx.hongshengwenyu.top

JS:   get name() { return this._name; }
来源：http://kmb.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://eie.shangyingyoupin.top

Java: public String getName() { return name; }
来源：http://ocf.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zvs.andypj.xyz

Ruby: attr_accessor :name
来源：http://tzq.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://gyy.bbcook.cn

[G12] 对象转字符串
来源：http://dyj.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://gci.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kxi.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://nwu.jqgufenzy.top

TS:   toString(): string { return this.name; }
来源：http://dxu.iojbl.cn

Java: @Override public String toString() { return name; }
来源：http://mrr.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://tpo.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://gvz.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://ego.nwbrower.top

[G13] 判断对象类型
来源：http://pmh.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://wul.snrcjt.cn

PHP:  $u instanceof User
来源：http://kkr.gogol.net.cn

JS:   u instanceof User
来源：http://kgq.jianghu66.top

TS:   u instanceof User
来源：http://vrn.guowangkeji.top

Java: u instanceof User
来源：http://exl.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://rox.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://ijt.yuanzhike.top

C#:   u is User
来源：http://nfm.52xcode.cn

[G14] 数据类 / record
来源：http://hvi.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gmr.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://cub.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gac.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://rit.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://sad.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://lvf.yj202588.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nde.yanxiufei.cn


<!-- 参考信息 -->