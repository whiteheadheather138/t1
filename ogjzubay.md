代发 wailian999

PHP:  number_format(1234567);
来源：http://cis.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://omc.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://hvj.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ghv.yj20258888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gta.shanyushiyangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ewf.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://lvd.c1oappe.top

[E17] 首字母大写
来源：http://aeq.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aoa.yonumen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hqd.jyoumei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tpy.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xsz.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://waw.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iiv.jianghu66.top

Ruby: s.capitalize
来源：http://zyv.dashuyun.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vgy.shuidangran.top

[E18] 模板占位符替换
来源：http://iyd.gaohongyu789.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jvj.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jxj.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cyn.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://aov.aibaodan.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kgm.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qji.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sfk.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ubn.snrcjt.cn

[E19] 多行文本按行拆分
来源：http://hgp.tian-w.cn

Py:   s.splitlines()
来源：http://igf.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jdc.nwbrower.top

JS:   s.split(/\r?\n/)
来源：http://aqy.shanyushiyangkeji.top

TS:   s.split(/\r?\n/)
来源：http://qdc.aibaodan.cn

Java: s.lines().toList()
来源：http://snh.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://iye.0kj1m.cn

Ruby: s.lines
来源：http://vnu.yanxiufei.cn

C#:   s.Split('\n')
来源：http://vnb.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://kho.yuanzhike.top

Py:   if not s:
来源：http://xdo.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dcc.hnqzz.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ewx.ybcxt.top

TS:   if (s === "") {}
来源：http://bjz.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://olc.aibaodan.cn

Go:   if s == "" {}
来源：http://lkf.guowangkeji.top

Ruby: if s.empty?
来源：http://vlm.smart0.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xed.hongshengwenyu.top

[E21] 超长截断加省略号
来源：http://iip.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tqc.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dte.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rhm.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kke.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iqv.xinyue.icu

Go:   // 按 rune 判断长度后截断
来源：http://fyr.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ant.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fnl.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://uew.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vnv.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gdu.wangdashe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xkl.yonumen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eyl.xylfe.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xef.meibo888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gvy.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://xki.yonumen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uyu.redwolf501.top

================================================================================
来源：http://gcf.ydzc1.top

F. 文件与目录
来源：http://xtm.jyoumei.cn

================================================================================
来源：http://oxv.bjfxy.top

[F01] 读取整个文件
来源：http://tyc.shuidangran.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xaa.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://hnm.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ewy.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pnb.zhaomingkeji.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://bwc.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://afk.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://tor.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://rix.cdnleiting.top

[F02] 逐行读取文件
来源：http://ame.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jcs.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://spi.cqqwz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://shv.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lcp.fanxiaobao.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xso.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fai.zdqjudy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ajz.52xcode.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qjc.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://juo.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dsv.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zxd.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bfe.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rtn.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://onj.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qea.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://wbg.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qaq.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://ejf.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qal.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://feu.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fmn.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://obs.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yoi.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gdp.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qoq.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rhz.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://uai.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pzh.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://ezh.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://wjv.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://soo.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://air.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kyn.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://mgg.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://sty.hfpthk.cn

[F06] 删除文件
来源：http://epo.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://ztr.bbcook.cn

PHP:  unlink("a.txt");
来源：http://bym.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://yjw.hongshengwenyu.top

TS:   fs.unlinkSync("a.txt")
来源：http://zxh.hongshengwenyu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://efm.9152youxi.cn

Go:   os.Remove("a.txt")
来源：http://jko.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://ett.xingfuxueyuan.xyz

C#:   File.Delete("a.txt");
来源：http://wzj.epnwcf.com

[F07] 创建目录（含多级）
来源：http://ayo.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tmv.feifeiyinyue.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zon.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dvs.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://shv.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yec.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rza.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ybf.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iba.sufxvd.cn

[F08] 遍历目录
来源：http://eds.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sok.jinqigfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gzk.xuetiantiany.cn

JS:   fs.readdirSync("dir")
来源：http://cgi.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://ahe.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ipm.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ike.zycfv.cn

Ruby: Dir.children("dir")
来源：http://spe.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://lmg.vehdjk.com

[F09] 获取文件大小
来源：http://hhh.hesvh.cn

Py:   os.path.getsize("a.txt")
来源：http://tti.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://ghd.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://war.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://tfm.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://nwh.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://meb.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://qca.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://omr.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://dse.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ied.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xxl.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dfk.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://cly.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lzr.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iha.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dkg.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vwy.xylfe.cn

[F11] 复制与移动文件
来源：http://fbm.yueranfly.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qiy.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nth.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lyt.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://spt.yj20258.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hfm.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://evk.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nnp.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rue.cucudq.cn

[F12] CSV 读写
来源：http://dhk.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dls.nwbrower.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lpf.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ftj.nanxuanxn.top

TS:   // 同上
来源：http://klp.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pjt.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://psa.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uqh.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uhh.haohaochexian.top

================================================================================
来源：http://ldc.jlsjyb.cn

G. 面向对象
来源：http://vbl.dianchejie.cn

================================================================================
来源：http://hux.smart0.xyz

[G01] 定义类
来源：http://tqz.cheryme.top

Py:   class User: pass
来源：http://twk.jiagoushi.top

PHP:  class User {}
来源：http://esm.gzhubu.top

JS:   class User {}
来源：http://dns.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://xjp.zdbjq.cn

Java: class User {}
来源：http://owr.uphjek.com

Go:   type User struct { Name string }
来源：http://lwp.jinghuilouyu.cn

Ruby: class User; end
来源：http://zwi.nanxinkj.top

C#:   class User {}
来源：http://cgf.xuanzx.com

[G02] 构造函数
来源：http://fin.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://zzq.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://bnj.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://rwa.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://nvv.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://sif.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://obc.hywenlv.cn

Ruby: def initialize(name); @name = name; end
来源：http://hml.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://wju.yuxming.cn

[G03] 实例属性
来源：http://ewo.chenzaomai.com

Py:   self.name = "x"
来源：http://tpf.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://zjd.hfpthk.cn

JS:   this.name = "x";
来源：http://cvq.iojbl.cn

TS:   name: string = "x";
来源：http://mtd.jqgfzy.top

Java: private String name;
来源：http://gtg.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wrz.tarul.cn

Ruby: @name = "x"
来源：http://wmh.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://pyb.yj20258888.top

[G04] 定义方法
来源：http://trs.xziqi.cn

Py:   def greet(self): return self.name
来源：http://zth.gotoacloud.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vcp.xinyue.icu

JS:   greet() { return this.name; }
来源：http://jah.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://mzk.nanxuanxn.top

Java: String greet() { return name; }
来源：http://ezp.wangshuangyany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rcz.9152youxi.cn

Ruby: def greet; @name; end
来源：http://deu.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://hwc.sysykeji.top

[G05] 继承
来源：http://ngt.chenlongwang.top

Py:   class Admin(User): pass
来源：http://wdp.shuidangran.top

PHP:  class Admin extends User {}
来源：http://cwj.ctjpmb.com

JS:   class Admin extends User {}
来源：http://xfm.hysaishi.cn

TS:   class Admin extends User {}
来源：http://jmh.wangdashe.top

Java: class Admin extends User {}
来源：http://btv.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://utj.yuanzhike.top

Ruby: class Admin < User; end
来源：http://izy.chenlongwang.top

C#:   class Admin : User {}
来源：http://dev.zhiwuduotai.top

[G06] 重写方法
来源：http://gbs.hywenlv.cn

Py:   def greet(self): return "admin"
来源：http://icc.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fxn.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://muv.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://ixa.tian-w.cn

Java: @Override String greet() { return "admin"; }
来源：http://pop.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hdk.zhixingplan.top

Ruby: def greet; "admin"; end
来源：http://nwy.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://hyi.svipenyu.cn

[G07] 调用父类方法
来源：http://dtl.zhongyouzk.top

Py:   super().greet()
来源：http://hmd.wangshuangyany.cn

PHP:  parent::greet();
来源：http://vwd.shanyushiyangtech.top

JS:   super.greet();
来源：http://rza.tanke756.top

TS:   super.greet();
来源：http://nmc.sufxvd.cn

Java: super.greet();
来源：http://eho.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xxu.hongshengwenyu.top

Ruby: super
来源：http://wgm.yangfankeji.com

C#:   base.Greet();
来源：http://bbq.cashguo.top

[G08] 静态方法与属性
来源：http://hbh.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ucc.birdmap.top

PHP:  public static function f() {}
来源：http://jmr.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://efv.iojbl.cn

TS:   static f(): void {}
来源：http://vyv.hammf.cn

Java: static void f() {}
来源：http://cly.chenzaomai.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://zzn.yj20258888.top

Ruby: def self.f; end
来源：http://qfj.nanxinkj.top

C#:   public static void F() {}
来源：http://rbm.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://toq.zycfv.cn

Py:   from abc import ABC, abstractmethod
来源：http://cmo.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://umt.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ptl.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://wto.zhongyouzk.top

Java: interface Shape { double area(); }
来源：http://ywa.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://uct.redwolf501.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ksz.sxryk.cn

C#:   interface IShape { double Area(); }
来源：http://upy.redwolf501.top

[G10] 访问控制
来源：http://nqv.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://mbq.gogol.net.cn

PHP:  public / protected / private
来源：http://yno.shuidangran.top

JS:   #private 字段；其余公开
来源：http://lwy.xuanzx.com

TS:   public / protected / private
来源：http://kxq.cashguo.top

Java: public / protected / private / 默认包级
来源：http://agp.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uhu.hongshengwenyu.top

Ruby: public / protected / private
来源：http://qpv.tian-w.cn

C#:   public / protected / private / internal
来源：http://fhz.gaohongyu789.top

[G11] getter / setter
来源：http://ams.sweek.top

Py:   @property 与 @x.setter
来源：http://tkz.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kwy.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://gfs.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://yoe.sufxvd.cn

Java: public String getName() { return name; }
来源：http://sgr.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://omf.hcnkem.com

Ruby: attr_accessor :name
来源：http://agg.yongpay.top

C#:   public string Name { get; set; }
来源：http://sxt.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://joz.jianghu66.top

Py:   def __str__(self): return self.name
来源：http://xwf.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://vmd.bbcook.cn

JS:   toString() { return this.name; }
来源：http://lyv.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://jnt.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://mtw.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://cox.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://ues.nanxuanxn.top

C#:   public override string ToString() => Name;
来源：http://vxh.hesvh.cn

[G13] 判断对象类型
来源：http://icw.shanyushiyangtech.top

Py:   isinstance(u, User)
来源：http://ghc.sjlbkw.cn

PHP:  $u instanceof User
来源：http://igk.shuidangran.top

JS:   u instanceof User
来源：http://muh.shangyingyoupin.top

TS:   u instanceof User
来源：http://zxa.yuxming.cn

Java: u instanceof User
来源：http://sdq.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gee.gzhubu.top

Ruby: u.is_a?(User)
来源：http://lmx.zhongyouzk.top

C#:   u is User
来源：http://ngb.kuanghao11.cn

[G14] 数据类 / record
来源：http://qru.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jse.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://bpz.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tzc.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://ies.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://cky.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://pii.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://krw.xinyue.icu


<!-- 参考信息 -->