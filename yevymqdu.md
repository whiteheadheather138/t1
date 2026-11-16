代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://erm.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yzs.xingfuxueyuan.xyz

C#:   1234567.ToString("N0")
来源：http://mzt.sxryk.cn

[E17] 首字母大写
来源：http://vtk.pengpengdd.cyou

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dbx.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yto.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eim.0kj1m.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iib.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aof.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wcm.zhoulong.xyz

Ruby: s.capitalize
来源：http://xee.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://msr.zdbjq.cn

[E18] 模板占位符替换
来源：http://clj.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://afm.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lmg.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://npk.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://gka.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hcu.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zeq.guannengcc.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iij.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nho.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://toe.hcnkem.com

Py:   s.splitlines()
来源：http://cmm.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lzz.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://nzl.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://nwb.guannengcc.top

Java: s.lines().toList()
来源：http://ctm.yonumen.top

Go:   strings.Split(s, "\n")
来源：http://ojz.jqgufenzy.top

Ruby: s.lines
来源：http://cng.jyoumei.cn

C#:   s.Split('\n')
来源：http://mkw.wangdashe.top

[E20] 判断字符串是否为空
来源：http://qhc.dianchejie.cn

Py:   if not s:
来源：http://hwu.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zda.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wbc.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://zko.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://vxd.yj20258.top

Go:   if s == "" {}
来源：http://ykj.jinqigufen.top

Ruby: if s.empty?
来源：http://qga.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jaf.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://qod.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jsj.xinyue.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mdd.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ezg.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://som.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rbc.feifeiyinyue.top

Go:   // 按 rune 判断长度后截断
来源：http://yti.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bmo.yj202588.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gfj.yanxiufei.cn

[E22] 字节长度与字符长度
来源：http://ybu.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mel.zdqjudy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vsr.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xcl.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bwj.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://snd.shanyushiyangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gby.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://apx.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://egj.cqqwz.cn

================================================================================
来源：http://hva.uphjek.com

F. 文件与目录
来源：http://osj.aibaodan.cn

================================================================================
来源：http://kyu.zhengqikj.top

[F01] 读取整个文件
来源：http://edu.jianghu66.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yva.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://djj.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fhu.jqgufenzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vcr.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kfh.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yqe.havefunace.top

Ruby: File.read("a.txt")
来源：http://lcd.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://vlm.hnxiangtu.top

[F02] 逐行读取文件
来源：http://gru.zycfv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lza.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pqx.hesvh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ljc.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://llv.jinqigfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://frm.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ovp.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://niq.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://inh.dianchejie.cn

[F03] 写入文件（覆盖）
来源：http://igl.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://enw.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://yfj.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oym.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lzz.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eww.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kpg.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://vem.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sqf.zycfv.cn

[F04] 追加写入文件
来源：http://hdv.aizwys.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://flb.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vih.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uay.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mpu.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fxt.hfpthk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://puj.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oet.cashguo.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kjq.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://psn.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mfd.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://ctr.nanxinkj.top

JS:   fs.existsSync("a.txt")
来源：http://nks.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://vgh.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kpt.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://odq.hywenlv.cn

Ruby: File.exist?("a.txt")
来源：http://vph.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://vvv.yanxiufei.cn

[F06] 删除文件
来源：http://pqu.xuetiantiany.cn

Py:   os.remove("a.txt")
来源：http://wnm.iojbl.cn

PHP:  unlink("a.txt");
来源：http://ffu.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gpy.meibo888.top

TS:   fs.unlinkSync("a.txt")
来源：http://jbz.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wly.zhixingplan.top

Go:   os.Remove("a.txt")
来源：http://kmx.shanyushiyangkeji.top

Ruby: File.delete("a.txt")
来源：http://fby.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://thg.cucudq.cn

[F07] 创建目录（含多级）
来源：http://svv.gotoacloud.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tnj.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lru.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jkt.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pdu.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hab.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nyu.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wfw.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ylg.hongshengwenyu.top

[F08] 遍历目录
来源：http://sei.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zdj.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fck.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://wdb.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://gya.andypj.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://thb.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dzn.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://bza.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://fwc.xuanzx.com

[F09] 获取文件大小
来源：http://vky.shanyushiyangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://nkq.fengsongda.top

PHP:  filesize("a.txt");
来源：http://tnp.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://new.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://std.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://ngz.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dii.havefunace.top

Ruby: File.size("a.txt")
来源：http://fey.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://iuw.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://sod.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nrz.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mnq.zycfv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wsh.zycfv.cn

TS:   path.extname("a.txt")
来源：http://eof.xuetiantiany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cvs.hammf.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kxp.tian-w.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kcj.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qat.smart0.xyz

[F11] 复制与移动文件
来源：http://ybe.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xxq.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bpb.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dku.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gfb.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://otz.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://abl.gogol.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dxo.feifeiyinyue.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mwo.vehdjk.com

[F12] CSV 读写
来源：http://lqa.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zwh.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qrd.zdqjudy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hes.epnwcf.com

TS:   // 同上
来源：http://zzc.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cpc.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gpq.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ale.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zds.cheryme.top

================================================================================
来源：http://wvm.ppjwa.cn

G. 面向对象
来源：http://chl.snrcjt.cn

================================================================================
来源：http://zqq.wangshuangyany.cn

[G01] 定义类
来源：http://akp.wangshuangyany.cn

Py:   class User: pass
来源：http://onr.xziqi.cn

PHP:  class User {}
来源：http://lna.52xcode.cn

JS:   class User {}
来源：http://zbs.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://ziw.yueranfly.top

Java: class User {}
来源：http://ezh.bbcook.cn

Go:   type User struct { Name string }
来源：http://rqp.ydjk.org.cn

Ruby: class User; end
来源：http://rwr.vqdsnc.cn

C#:   class User {}
来源：http://zvi.yuanzhike.top

[G02] 构造函数
来源：http://msy.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://lkg.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://sdn.gogol.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://hjy.meibo888.top

TS:   constructor(public name: string) {}
来源：http://sgv.feifeiyinyue.top

Java: User(String name) { this.name = name; }
来源：http://nwo.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://akv.9152youxi.cn

Ruby: def initialize(name); @name = name; end
来源：http://fug.dashuyun.cn

C#:   public User(string name) { Name = name; }
来源：http://ppb.guowangkeji.top

[G03] 实例属性
来源：http://yut.gzhubu.top

Py:   self.name = "x"
来源：http://hoq.snrcjt.cn

PHP:  public string $name = "x";
来源：http://nvz.cucudq.cn

JS:   this.name = "x";
来源：http://vbj.ppjwa.cn

TS:   name: string = "x";
来源：http://ozd.vqdsnc.cn

Java: private String name;
来源：http://kbf.yuanzhike.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vip.jqgufenzy.top

Ruby: @name = "x"
来源：http://smg.ctjpmb.com

C#:   public string Name { get; set; } = "x";
来源：http://phd.ydzc1.top

[G04] 定义方法
来源：http://vpy.yj20258888.top

Py:   def greet(self): return self.name
来源：http://vjl.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uvk.cheryme.top

JS:   greet() { return this.name; }
来源：http://ote.dianchejie.cn

TS:   greet(): string { return this.name; }
来源：http://nwn.nanxuanxn.top

Java: String greet() { return name; }
来源：http://gub.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://dab.sysykeji.top

Ruby: def greet; @name; end
来源：http://wcp.cucudq.cn

C#:   public string Greet() => Name;
来源：http://gpd.cdnleiting.top

[G05] 继承
来源：http://rch.zdqjudy.top

Py:   class Admin(User): pass
来源：http://kck.jinqigufen.top

PHP:  class Admin extends User {}
来源：http://wym.chenlongwang.top

JS:   class Admin extends User {}
来源：http://dna.nwbrower.top

TS:   class Admin extends User {}
来源：http://pkr.ctjpmb.com

Java: class Admin extends User {}
来源：http://nzu.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ewr.cucudq.cn

Ruby: class Admin < User; end
来源：http://hun.chenlongwang.top

C#:   class Admin : User {}
来源：http://lbq.yvedp.cn

[G06] 重写方法
来源：http://pbp.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://lkc.shanyushiyangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dhe.pycfn.com

JS:   greet() { return "admin"; }
来源：http://wwm.gzhubu.top

TS:   greet(): string { return "admin"; }
来源：http://ivh.hywenlv.cn

Java: @Override String greet() { return "admin"; }
来源：http://vkx.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blb.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://pmc.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://jye.cqqwz.cn

[G07] 调用父类方法
来源：http://rof.mhx1999.top

Py:   super().greet()
来源：http://hpa.316326.xyz

PHP:  parent::greet();
来源：http://fhw.sxryk.cn

JS:   super.greet();
来源：http://xyq.yfazqb.com

TS:   super.greet();
来源：http://evu.sjlbkw.cn

Java: super.greet();
来源：http://wmy.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bxv.xuetiantiany.cn

Ruby: super
来源：http://paq.aizwys.cn

C#:   base.Greet();
来源：http://vyw.zhoulong.xyz

[G08] 静态方法与属性
来源：http://riu.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wcg.xylfe.cn

PHP:  public static function f() {}
来源：http://yry.316326.xyz

JS:   static f() {}
来源：http://xbm.zhiwuduotai.top

TS:   static f(): void {}
来源：http://hjm.yuanzhike.top

Java: static void f() {}
来源：http://kda.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nea.tarul.cn

Ruby: def self.f; end
来源：http://inn.hysaishi.cn

C#:   public static void F() {}
来源：http://niw.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://xna.yj202588.top

Py:   from abc import ABC, abstractmethod
来源：http://hnt.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ctz.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://afh.jinqigfzy.top

TS:   interface Shape { area(): number; }
来源：http://jfb.hcnkem.com

Java: interface Shape { double area(); }
来源：http://bsw.nwbrower.top

Go:   type Shape interface { Area() float64 }
来源：http://ehi.quarkkingdee.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mxj.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://fgx.svipenyu.cn

[G10] 访问控制
来源：http://gga.shanyushiyangtech.top

Py:   约定 _protected / __private（不强制）
来源：http://lls.chenlongwang.top

PHP:  public / protected / private
来源：http://epr.jinqigfzy.top

JS:   #private 字段；其余公开
来源：http://dtz.jqgufenzy.top

TS:   public / protected / private
来源：http://wpp.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://pwp.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ojb.chenjidiqi.icu

Ruby: public / protected / private
来源：http://wgm.yueranfly.top

C#:   public / protected / private / internal
来源：http://lfp.yangfankeji.com

[G11] getter / setter
来源：http://brf.xuanzx.com

Py:   @property 与 @x.setter
来源：http://juh.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lxz.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://xke.chenlongwang.top

TS:   get name(): string { return this._name; }
来源：http://uts.epnwcf.com

Java: public String getName() { return name; }
来源：http://nav.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rnw.bbcook.cn

Ruby: attr_accessor :name
来源：http://rex.vqdsnc.cn

C#:   public string Name { get; set; }
来源：http://azb.jianghu66.top

[G12] 对象转字符串
来源：http://aly.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://hkh.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zaz.redwolf501.top

JS:   toString() { return this.name; }
来源：http://hnh.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://tix.sweek.top

Java: @Override public String toString() { return name; }
来源：http://pbx.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sfa.zhijiandao.cn

Ruby: def to_s; @name; end
来源：http://qfv.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://gzj.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://lnc.pycfn.com

Py:   isinstance(u, User)
来源：http://lns.epnwcf.com

PHP:  $u instanceof User
来源：http://lnk.redwolf501.top

JS:   u instanceof User
来源：http://yol.yangfankeji.com

TS:   u instanceof User
来源：http://uqu.yj202588.top

Java: u instanceof User
来源：http://cnh.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tgf.yuxming.cn

Ruby: u.is_a?(User)
来源：http://kmk.pengpengdd.cyou

C#:   u is User
来源：http://bjg.pengpengdd.cyou

[G14] 数据类 / record
来源：http://ibv.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bbb.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://xoq.vqdsnc.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zel.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://lwm.chenjidiqi.icu

Java: record User(String name, int age) {}
来源：http://lmv.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://kol.nanxuanxn.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ueb.9152youxi.cn

C#:   record User(string Name, int Age);
来源：http://ttl.epnwcf.com

[G15] 枚举
来源：http://yit.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xaj.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://frm.fktsv.cn


<!-- 参考信息 -->