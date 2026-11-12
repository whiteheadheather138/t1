代发 wailian999

PHP:  number_format(1234567);
来源：http://xjd.zhijiandao.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zlp.xinyue.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://szx.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qhd.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://btq.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bxx.xinyue.icu

C#:   1234567.ToString("N0")
来源：http://ftx.yuanzhike.top

[E17] 首字母大写
来源：http://ofn.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cqm.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pbr.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nse.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rxu.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zbz.zycfv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jee.yongpay.top

Ruby: s.capitalize
来源：http://ifa.xuetiantiany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iat.shzxlz.cn

[E18] 模板占位符替换
来源：http://dhc.xziqi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://chd.wangshuangyany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rpr.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qdg.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bpm.chenjidiqi.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hmg.yj20258888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cqp.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://axo.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ger.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://fuu.zycfv.cn

Py:   s.splitlines()
来源：http://kge.jinqigfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yaj.cucudq.cn

JS:   s.split(/\r?\n/)
来源：http://fcw.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://zpm.xziqi.cn

Java: s.lines().toList()
来源：http://adc.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://gym.haohaochexian.top

Ruby: s.lines
来源：http://qti.tanke756.top

C#:   s.Split('\n')
来源：http://vao.52xcode.cn

[E20] 判断字符串是否为空
来源：http://ohg.svipenyu.cn

Py:   if not s:
来源：http://itd.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fpb.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://edx.yueranfly.top

TS:   if (s === "") {}
来源：http://iep.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://kyp.uphjek.com

Go:   if s == "" {}
来源：http://jvu.shangyingyoupin.top

Ruby: if s.empty?
来源：http://xrf.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hih.yj202588.top

[E21] 超长截断加省略号
来源：http://txz.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eyj.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yyt.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gyx.jlsjyb.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yon.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://etn.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://zkf.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ddh.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ycj.316326.xyz

[E22] 字节长度与字符长度
来源：http://eou.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lmf.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://acv.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vvh.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jec.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yfa.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uzr.fehbvm.com

Ruby: s.bytesize;  s.length
来源：http://muy.9152youxi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rbx.ydzc1.top

================================================================================
来源：http://wwl.cdnleiting.top

F. 文件与目录
来源：http://fvq.mhx1999.top

================================================================================
来源：http://wbd.shzxlz.cn

[F01] 读取整个文件
来源：http://dyt.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fhd.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://xef.jqgfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qal.yj20258.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uie.jyoumei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xmy.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://out.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://djj.yuxming.cn

C#:   File.ReadAllText("a.txt");
来源：http://yui.quarkkingdee.top

[F02] 逐行读取文件
来源：http://lqd.hnqzz.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://glq.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vcv.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rbd.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://usc.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vht.cqqwz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pap.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fpv.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qie.pycfn.com

[F03] 写入文件（覆盖）
来源：http://cjr.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rdx.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mys.nanxuanxn.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://weo.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xfq.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vwc.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uiv.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://szy.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tbj.tianlin.xyz

[F04] 追加写入文件
来源：http://dop.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hwh.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iii.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vne.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xiq.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aaq.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wsm.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ztg.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nyf.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://gqj.hammf.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yyp.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://lux.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://mzb.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://yvd.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wgf.kuanghao11.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gxk.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://iob.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://zfv.sjlbkw.cn

[F06] 删除文件
来源：http://zhp.guannengcc.top

Py:   os.remove("a.txt")
来源：http://hnc.yueranfly.top

PHP:  unlink("a.txt");
来源：http://vld.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://jpq.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://ylx.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gvx.zhiwuduotai.top

Go:   os.Remove("a.txt")
来源：http://rvu.smart0.xyz

Ruby: File.delete("a.txt")
来源：http://abt.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://zkr.ctjpmb.com

[F07] 创建目录（含多级）
来源：http://qfm.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ylj.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mcu.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oog.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fts.sweek.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qth.tian-w.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://myo.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ird.aibaodan.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hfz.xylfe.cn

[F08] 遍历目录
来源：http://qnm.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wse.zdbjq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zon.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://eic.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://wpw.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aem.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gmj.hfpthk.cn

Ruby: Dir.children("dir")
来源：http://sbf.zhoulong.xyz

C#:   Directory.GetFiles("dir")
来源：http://awi.zhijiandao.cn

[F09] 获取文件大小
来源：http://stj.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://vdp.nanxinkj.top

PHP:  filesize("a.txt");
来源：http://oct.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://aja.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://gcn.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vxp.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hua.havefunace.top

Ruby: File.size("a.txt")
来源：http://ghg.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://snh.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://uvx.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tkl.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gzh.sjlbkw.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ojv.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://ewl.shangyingyoupin.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ugk.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gyd.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bxo.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qan.hnxiangtu.top

[F11] 复制与移动文件
来源：http://ydn.yvedp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://acf.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qer.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uhu.zdqjudy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nfq.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ljf.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qhc.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dig.havefunace.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pbx.hywenlv.cn

[F12] CSV 读写
来源：http://dni.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mgf.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ewe.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wmm.chenlongwang.top

TS:   // 同上
来源：http://piu.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://avx.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ruf.dashuyun.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jhi.shzxlz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xpo.andypj.xyz

================================================================================
来源：http://vnm.cheryme.top

G. 面向对象
来源：http://qat.ppjwa.cn

================================================================================
来源：http://wnk.jinyuanbaomall.cn

[G01] 定义类
来源：http://imo.cheryme.top

Py:   class User: pass
来源：http://oxf.yonumen.top

PHP:  class User {}
来源：http://wvi.tanke756.top

JS:   class User {}
来源：http://uji.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://siw.cqqwz.cn

Java: class User {}
来源：http://fcx.jianghu66.top

Go:   type User struct { Name string }
来源：http://hho.guannengcc.top

Ruby: class User; end
来源：http://eut.birdmap.top

C#:   class User {}
来源：http://dou.hywenlv.cn

[G02] 构造函数
来源：http://suw.0kj1m.cn

Py:   def __init__(self, name): self.name = name
来源：http://rqg.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://zve.fehbvm.com

JS:   constructor(name) { this.name = name; }
来源：http://vbt.daxiang520.top

TS:   constructor(public name: string) {}
来源：http://vgn.chenzaomai.com

Java: User(String name) { this.name = name; }
来源：http://rox.hesvh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qrv.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://dic.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://zsf.ctjpmb.com

[G03] 实例属性
来源：http://whe.aibaodan.cn

Py:   self.name = "x"
来源：http://mjn.dashuyun.cn

PHP:  public string $name = "x";
来源：http://pem.zhixingplan.top

JS:   this.name = "x";
来源：http://tim.yueranfly.top

TS:   name: string = "x";
来源：http://cwh.sysykeji.top

Java: private String name;
来源：http://uxj.zhijiandao.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://upk.ydjk.org.cn

Ruby: @name = "x"
来源：http://mfd.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://iuy.shzxlz.cn

[G04] 定义方法
来源：http://jgc.daria6918.cn

Py:   def greet(self): return self.name
来源：http://pca.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fkl.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://ird.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://umv.aizwys.cn

Java: String greet() { return name; }
来源：http://gki.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lkz.snrcjt.cn

Ruby: def greet; @name; end
来源：http://ghl.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://flj.fengsongda.top

[G05] 继承
来源：http://cjf.guowangkeji.top

Py:   class Admin(User): pass
来源：http://utb.ppjwa.cn

PHP:  class Admin extends User {}
来源：http://aoi.guannengcc.top

JS:   class Admin extends User {}
来源：http://bjn.mhx1999.top

TS:   class Admin extends User {}
来源：http://faq.nanxinkj.top

Java: class Admin extends User {}
来源：http://cut.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gpk.jqgfzy.top

Ruby: class Admin < User; end
来源：http://dvg.zhongyouzk.top

C#:   class Admin : User {}
来源：http://dyp.ehwqpu.com

[G06] 重写方法
来源：http://vnk.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://qfz.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://uvc.pycfn.com

JS:   greet() { return "admin"; }
来源：http://ajo.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://cxt.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://wcp.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ddk.zdbjq.cn

Ruby: def greet; "admin"; end
来源：http://zrf.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://nxd.chenjidiqi.icu

[G07] 调用父类方法
来源：http://tbq.chenjidiqi.icu

Py:   super().greet()
来源：http://wuq.yanxiufei.cn

PHP:  parent::greet();
来源：http://cox.xylfe.cn

JS:   super.greet();
来源：http://lmy.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://hvd.cashguo.top

Java: super.greet();
来源：http://oao.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://juc.gaohongyu789.top

Ruby: super
来源：http://tgn.gzhubu.top

C#:   base.Greet();
来源：http://kvj.zhoulong.xyz

[G08] 静态方法与属性
来源：http://fmz.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gst.ybcxt.top

PHP:  public static function f() {}
来源：http://plp.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://okj.bjfxy.top

TS:   static f(): void {}
来源：http://yub.svipenyu.cn

Java: static void f() {}
来源：http://sdn.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ipi.kuanghao11.cn

Ruby: def self.f; end
来源：http://yac.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://qhf.daria6918.cn

[G09] 接口 / 抽象类
来源：http://fqu.nwbrower.top

Py:   from abc import ABC, abstractmethod
来源：http://mus.wangshuangyany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ypd.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zxs.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://tmx.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://chf.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://kqw.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rbu.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://zlm.zhixingplan.top

[G10] 访问控制
来源：http://tij.zhongyouzk.top

Py:   约定 _protected / __private（不强制）
来源：http://wmm.fktsv.cn

PHP:  public / protected / private
来源：http://kfl.meibo888.top

JS:   #private 字段；其余公开
来源：http://crs.nanxuanxn.top

TS:   public / protected / private
来源：http://qrk.uphjek.com

Java: public / protected / private / 默认包级
来源：http://mgt.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lkq.wangshuangyany.cn

Ruby: public / protected / private
来源：http://jxt.fengsongda.top

C#:   public / protected / private / internal
来源：http://mrz.yj20258888.top

[G11] getter / setter
来源：http://fvr.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://eoy.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dfx.tarul.cn

JS:   get name() { return this._name; }
来源：http://jdt.aizwys.cn

TS:   get name(): string { return this._name; }
来源：http://gzx.hcnkem.com

Java: public String getName() { return name; }
来源：http://ank.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://rnq.snrcjt.cn

Ruby: attr_accessor :name
来源：http://juo.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://nti.xuetiantiany.cn

[G12] 对象转字符串
来源：http://hxg.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://fck.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pku.yueranfly.top

JS:   toString() { return this.name; }
来源：http://qzh.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://rrb.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://nsa.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://gkd.fengsongda.top

Ruby: def to_s; @name; end
来源：http://msr.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://ifa.sufxvd.cn

[G13] 判断对象类型
来源：http://hve.tarul.cn

Py:   isinstance(u, User)
来源：http://nvw.tarul.cn

PHP:  $u instanceof User
来源：http://cel.cqqwz.cn

JS:   u instanceof User
来源：http://xab.vehdjk.com

TS:   u instanceof User
来源：http://gqm.hfpthk.cn

Java: u instanceof User
来源：http://jsf.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://crk.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://czx.jinqigfzy.top

C#:   u is User
来源：http://nur.52xcode.cn

[G14] 数据类 / record
来源：http://rfn.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nuv.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://fzq.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://des.shangyingyoupin.top

TS:   type User = { name: string; age: number };
来源：http://cov.mhx1999.top

Java: record User(String name, int age) {}
来源：http://xkb.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://qld.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wyx.pengpengdd.cyou


<!-- 参考信息 -->