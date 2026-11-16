代发 wailian999

PHP:  number_format(1234567);
来源：http://cxa.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://uyh.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jne.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zyi.sxryk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xao.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uoq.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://ixh.guannengcc.top

[E17] 首字母大写
来源：http://lgc.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dlj.shanyushiyangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bmh.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://deu.gzhubu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://exj.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ykp.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ghd.shuidangran.top

Ruby: s.capitalize
来源：http://smu.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mio.shuidangran.top

[E18] 模板占位符替换
来源：http://ilj.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zgp.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qlz.pycfn.com

JS:   tpl.replaceAll("{name}", name)
来源：http://qac.svipenyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bmv.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://env.nwbrower.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://diz.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kgw.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nor.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://pwi.kuanghao11.cn

Py:   s.splitlines()
来源：http://jzi.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jnn.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://fxo.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://eyt.fehbvm.com

Java: s.lines().toList()
来源：http://kwa.sweek.top

Go:   strings.Split(s, "\n")
来源：http://isk.nwbrower.top

Ruby: s.lines
来源：http://qbj.hcnkem.com

C#:   s.Split('\n')
来源：http://ydo.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://grl.hfpthk.cn

Py:   if not s:
来源：http://cro.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hrv.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qjd.quarkkingdee.top

TS:   if (s === "") {}
来源：http://mch.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://cxy.chenlongwang.top

Go:   if s == "" {}
来源：http://sxw.hcnkem.com

Ruby: if s.empty?
来源：http://iwj.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://the.ivvv.top

[E21] 超长截断加省略号
来源：http://fsf.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vxl.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gvo.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jis.jlsjyb.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://umi.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gzw.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://mjs.pycfn.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qyx.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vod.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://bvf.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cvo.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sqf.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ehl.zhiwuduotai.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://keh.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xdg.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xng.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://mzj.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rjd.hysaishi.cn

================================================================================
来源：http://cqx.xingfuxueyuan.xyz

F. 文件与目录
来源：http://hzd.cashguo.top

================================================================================
来源：http://mam.ehwqpu.com

[F01] 读取整个文件
来源：http://sgi.xziqi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wvk.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://bos.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eor.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ogw.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://obk.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://his.ybcxt.top

Ruby: File.read("a.txt")
来源：http://ehd.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://gxo.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://xpp.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mse.bjfxy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uif.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ixj.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vcm.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wdz.gogol.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aua.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dgp.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gjc.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://sft.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lvz.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jqa.jinqigufen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xxp.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dwz.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fyk.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bzp.chenjidiqi.icu

Ruby: File.write("a.txt", "hi")
来源：http://ucj.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yuw.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://bwe.zdqjudy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xtu.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vgc.fanxiaobao.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lje.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hyh.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jjb.zhiwuduotai.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rut.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zez.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lgh.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://flj.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lrd.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://oyf.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://wkg.kuanghao11.cn

TS:   fs.existsSync("a.txt")
来源：http://wnx.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://plh.ivvv.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gkg.tarul.cn

Ruby: File.exist?("a.txt")
来源：http://dis.shzxlz.cn

C#:   File.Exists("a.txt")
来源：http://mhm.tanke756.top

[F06] 删除文件
来源：http://cxn.jiagoushi.top

Py:   os.remove("a.txt")
来源：http://eud.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://xpb.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tjo.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://moz.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xoa.smart0.xyz

Go:   os.Remove("a.txt")
来源：http://hyv.zhaomingkeji.xyz

Ruby: File.delete("a.txt")
来源：http://gnu.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://qzb.yonumen.top

[F07] 创建目录（含多级）
来源：http://cmj.guannengcc.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zqe.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zvx.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://szh.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qqe.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wwb.yuanzhike.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ith.xuanzx.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xmj.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pnt.pengpengdd.cyou

[F08] 遍历目录
来源：http://kkd.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ecp.zycfv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://din.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://yee.zhaomingkeji.xyz

TS:   fs.readdirSync("dir")
来源：http://kpi.redwolf501.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://muq.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://fdb.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://com.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://heb.chenjidiqi.icu

[F09] 获取文件大小
来源：http://hnk.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://zal.tanke756.top

PHP:  filesize("a.txt");
来源：http://jiw.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://ilg.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://xyq.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gsb.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vqu.tanke756.top

Ruby: File.size("a.txt")
来源：http://gbj.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://zcz.ywan-chungtsiang.top

[F10] 取文件扩展名 / 文件名
来源：http://hao.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rge.gotoacloud.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uyx.52xcode.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rnm.yuxming.cn

TS:   path.extname("a.txt")
来源：http://niw.zhijiandao.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://urg.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dgk.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fus.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fvt.hnxiangtu.top

[F11] 复制与移动文件
来源：http://tfr.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oex.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ang.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mnz.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qdg.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mmx.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://txw.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tis.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://okf.yj20258.top

[F12] CSV 读写
来源：http://hct.tian-w.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oko.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hqa.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://poq.sxryk.cn

TS:   // 同上
来源：http://zys.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://etl.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ufu.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ivm.shanyushiyangtech.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pdr.zdqjudy.top

================================================================================
来源：http://mik.ywan-chungtsiang.top

G. 面向对象
来源：http://ysy.yueranfly.top

================================================================================
来源：http://ban.tianlin.xyz

[G01] 定义类
来源：http://pjp.yuanzhike.top

Py:   class User: pass
来源：http://hpa.snrcjt.cn

PHP:  class User {}
来源：http://nxr.gzhubu.top

JS:   class User {}
来源：http://hze.yvedp.cn

TS:   class User { name: string = ""; }
来源：http://gnf.ybcxt.top

Java: class User {}
来源：http://hgd.xuanzx.com

Go:   type User struct { Name string }
来源：http://fzi.yueranfly.top

Ruby: class User; end
来源：http://qux.jinqigufen.top

C#:   class User {}
来源：http://klc.0kj1m.cn

[G02] 构造函数
来源：http://ssc.ydzc1.top

Py:   def __init__(self, name): self.name = name
来源：http://haz.guannengcc.top

PHP:  public function __construct(public string $name) {}
来源：http://xcu.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://fkg.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://lnb.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://baq.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lit.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://mko.svipenyu.cn

C#:   public User(string name) { Name = name; }
来源：http://mcu.feifeiyinyue.top

[G03] 实例属性
来源：http://phq.jyoumei.cn

Py:   self.name = "x"
来源：http://lxa.sweek.top

PHP:  public string $name = "x";
来源：http://hmt.tian-w.cn

JS:   this.name = "x";
来源：http://dxq.redwolf501.top

TS:   name: string = "x";
来源：http://vzf.hnxiangtu.top

Java: private String name;
来源：http://tuc.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wwo.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://zjr.zdqjudy.top

C#:   public string Name { get; set; } = "x";
来源：http://sbd.yanxiufei.cn

[G04] 定义方法
来源：http://wlz.epnwcf.com

Py:   def greet(self): return self.name
来源：http://oho.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rfw.yuanzhike.top

JS:   greet() { return this.name; }
来源：http://kdo.jinqigfzy.top

TS:   greet(): string { return this.name; }
来源：http://oqv.yj202588.top

Java: String greet() { return name; }
来源：http://hqn.xuanzx.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://udm.yvedp.cn

Ruby: def greet; @name; end
来源：http://ect.smart0.xyz

C#:   public string Greet() => Name;
来源：http://pmi.hammf.cn

[G05] 继承
来源：http://rwt.andypj.xyz

Py:   class Admin(User): pass
来源：http://uab.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://uwz.snrcjt.cn

JS:   class Admin extends User {}
来源：http://wfk.tarul.cn

TS:   class Admin extends User {}
来源：http://bvw.fehbvm.com

Java: class Admin extends User {}
来源：http://kym.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://krq.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://har.sjlbkw.cn

C#:   class Admin : User {}
来源：http://jyw.52xcode.cn

[G06] 重写方法
来源：http://tzq.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://cyi.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yjf.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://ito.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://dgj.hfpthk.cn

Java: @Override String greet() { return "admin"; }
来源：http://qat.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jfj.fktsv.cn

Ruby: def greet; "admin"; end
来源：http://elt.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://ncu.xylfe.cn

[G07] 调用父类方法
来源：http://wto.meibo888.top

Py:   super().greet()
来源：http://uzp.yfazqb.com

PHP:  parent::greet();
来源：http://cog.tanke756.top

JS:   super.greet();
来源：http://byp.tian-w.cn

TS:   super.greet();
来源：http://iiv.guannengcc.top

Java: super.greet();
来源：http://ssj.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gwj.sweek.top

Ruby: super
来源：http://omp.tanke756.top

C#:   base.Greet();
来源：http://rxx.yuxming.cn

[G08] 静态方法与属性
来源：http://obh.jlsjyb.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tni.shzxlz.cn

PHP:  public static function f() {}
来源：http://ark.cqqwz.cn

JS:   static f() {}
来源：http://mtj.9152youxi.cn

TS:   static f(): void {}
来源：http://xmk.hywenlv.cn

Java: static void f() {}
来源：http://gog.gogol.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zgf.gogol.net.cn

Ruby: def self.f; end
来源：http://sgu.jinqigufen.top

C#:   public static void F() {}
来源：http://ixb.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://ily.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://tjr.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fuw.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bsa.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://oac.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://mla.wangshuangyany.cn

Go:   type Shape interface { Area() float64 }
来源：http://vhl.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vrl.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://jjg.mhx1999.top

[G10] 访问控制
来源：http://dts.xuetiantiany.cn

Py:   约定 _protected / __private（不强制）
来源：http://mbx.hnxiangtu.top

PHP:  public / protected / private
来源：http://dtx.epnwcf.com

JS:   #private 字段；其余公开
来源：http://cqe.zdqjudy.top

TS:   public / protected / private
来源：http://vsr.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://ugu.epnwcf.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://cyw.yongpay.top

Ruby: public / protected / private
来源：http://qfn.epnwcf.com

C#:   public / protected / private / internal
来源：http://zws.316326.xyz

[G11] getter / setter
来源：http://fgs.epnwcf.com

Py:   @property 与 @x.setter
来源：http://uql.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://drh.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://wps.yj20258.top

TS:   get name(): string { return this._name; }
来源：http://ffy.hywenlv.cn

Java: public String getName() { return name; }
来源：http://plm.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zgm.sxryk.cn

Ruby: attr_accessor :name
来源：http://gsb.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://pew.guannengcc.top

[G12] 对象转字符串
来源：http://oph.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://pix.pycfn.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://sdv.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://blm.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://gdu.shuidangran.top

Java: @Override public String toString() { return name; }
来源：http://njz.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lqq.ydzc1.top

Ruby: def to_s; @name; end
来源：http://mrp.snrcjt.cn

C#:   public override string ToString() => Name;
来源：http://tol.yj20258.top

[G13] 判断对象类型
来源：http://giw.yj20258.top

Py:   isinstance(u, User)
来源：http://ziv.gzhubu.top

PHP:  $u instanceof User
来源：http://izg.epnwcf.com

JS:   u instanceof User
来源：http://vvt.zycfv.cn

TS:   u instanceof User
来源：http://peb.cashguo.top

Java: u instanceof User
来源：http://szj.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aqn.uphjek.com

Ruby: u.is_a?(User)
来源：http://jnk.kuanghao11.cn

C#:   u is User
来源：http://omn.xylfe.cn

[G14] 数据类 / record
来源：http://aek.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hdx.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://owx.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hec.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://npc.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://btz.hywenlv.cn

Go:   type User struct { Name string; Age int }
来源：http://vtz.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wqj.ehwqpu.com


<!-- 参考信息 -->