代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wbe.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mwg.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://woa.hammf.cn

[E17] 首字母大写
来源：http://zjv.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bbk.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://nit.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lup.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gkk.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xpt.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hhv.jlsjyb.cn

Ruby: s.capitalize
来源：http://aoi.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jkc.shanyushiyangkeji.top

[E18] 模板占位符替换
来源：http://aop.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://chy.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pir.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://chn.iojbl.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jwa.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wep.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oqt.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://olv.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hdb.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://yhs.nanxuanxn.top

Py:   s.splitlines()
来源：http://scb.fzhhl.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://npl.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://zly.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://gsf.gaohongyu789.top

Java: s.lines().toList()
来源：http://fai.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://ewi.kuanghao11.cn

Ruby: s.lines
来源：http://kek.gzhubu.top

C#:   s.Split('\n')
来源：http://swz.sxryk.cn

[E20] 判断字符串是否为空
来源：http://zmt.fanxiaobao.xyz

Py:   if not s:
来源：http://yom.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xsg.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dpm.wangdashe.top

TS:   if (s === "") {}
来源：http://six.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://arf.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://gdl.feifeiyinyue.top

Ruby: if s.empty?
来源：http://qmj.xziqi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dzo.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://fyg.chenlongwang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wpa.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dnx.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://szp.zhoulong.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://clx.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://spx.ehwqpu.com

Go:   // 按 rune 判断长度后截断
来源：http://yue.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tga.ivvv.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://isu.bbcook.cn

[E22] 字节长度与字符长度
来源：http://bop.haohaochexian.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bgl.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wyp.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://por.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lmv.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jvs.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ykt.zdqjudy.top

Ruby: s.bytesize;  s.length
来源：http://lvh.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://upo.cucudq.cn

================================================================================
来源：http://sqa.chenjidiqi.icu

F. 文件与目录
来源：http://uke.wangshuangyany.cn

================================================================================
来源：http://dxs.chenjidiqi.icu

[F01] 读取整个文件
来源：http://raj.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yrq.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://bec.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://asq.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://llg.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ffe.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iel.meibo888.top

Ruby: File.read("a.txt")
来源：http://rsi.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://jqi.guannengcc.top

[F02] 逐行读取文件
来源：http://ibm.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bpn.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jvu.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vhg.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://smz.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bth.gogol.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iwc.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mfw.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bzu.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://qmg.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cfb.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mzp.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nqz.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dgb.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dvy.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cyo.hcnkem.com

Ruby: File.write("a.txt", "hi")
来源：http://pvn.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ltq.hnqzz.top

[F04] 追加写入文件
来源：http://owf.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vts.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wcj.ydjk.org.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://clz.daxiang520.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://grp.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wdy.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fbo.aibaodan.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ngp.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pxx.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://jli.zhoulong.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://klo.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://nnr.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://nef.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://nop.sysykeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zjr.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fhk.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://xwb.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://szo.zycfv.cn

[F06] 删除文件
来源：http://jxh.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://kzg.yongpay.top

PHP:  unlink("a.txt");
来源：http://jkz.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://bvl.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://msj.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pnc.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://xcs.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://qjk.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://rxq.cucudq.cn

[F07] 创建目录（含多级）
来源：http://vxr.nanxinkj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ulh.shanyushiyangtech.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uyv.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://guu.chenlongwang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://swg.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xku.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tcz.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ucm.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xgt.hnqzz.top

[F08] 遍历目录
来源：http://rhz.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vzu.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tbh.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://igh.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://kes.ybcxt.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sun.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hbs.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://jbx.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://qlr.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://asv.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://iva.bjfxy.top

PHP:  filesize("a.txt");
来源：http://dps.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://erk.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://rxe.yfazqb.com

Java: Files.size(Path.of("a.txt"))
来源：http://aft.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://stm.uphjek.com

Ruby: File.size("a.txt")
来源：http://uyk.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://svt.dashuyun.cn

[F10] 取文件扩展名 / 文件名
来源：http://aix.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gfr.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dsf.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nkm.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://dmb.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://afd.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vyu.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://afi.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vvo.hammf.cn

[F11] 复制与移动文件
来源：http://fwu.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vuw.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://low.xuanzx.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://abk.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dfe.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gco.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://goi.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ufi.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cyz.hnqzz.top

[F12] CSV 读写
来源：http://uff.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dnq.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eyk.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pll.316326.xyz

TS:   // 同上
来源：http://iig.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kls.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://csv.jinqigufen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://npe.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wyv.jianghu66.top

================================================================================
来源：http://lwe.aibaodan.cn

G. 面向对象
来源：http://wwv.svipenyu.cn

================================================================================
来源：http://dwc.jinyuanbaomall.cn

[G01] 定义类
来源：http://hqh.hywenlv.cn

Py:   class User: pass
来源：http://wdu.chenlongwang.top

PHP:  class User {}
来源：http://ryy.zdqjudy.top

JS:   class User {}
来源：http://eny.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://qud.fanxiaobao.xyz

Java: class User {}
来源：http://vqu.ybcxt.top

Go:   type User struct { Name string }
来源：http://edo.yj20258.top

Ruby: class User; end
来源：http://lop.chenlongwang.top

C#:   class User {}
来源：http://cvw.jlsjyb.cn

[G02] 构造函数
来源：http://lwt.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://guc.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://zbn.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://fpf.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://cld.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://gdg.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mts.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://taa.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://rsp.gotoacloud.top

[G03] 实例属性
来源：http://tqg.ehwqpu.com

Py:   self.name = "x"
来源：http://sgp.redwolf501.top

PHP:  public string $name = "x";
来源：http://nsp.zhengqikj.top

JS:   this.name = "x";
来源：http://hxg.iojbl.cn

TS:   name: string = "x";
来源：http://avo.jinyuanbaomall.cn

Java: private String name;
来源：http://dtg.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eeh.ybcxt.top

Ruby: @name = "x"
来源：http://txv.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://own.xziqi.cn

[G04] 定义方法
来源：http://zcu.hnxiangtu.top

Py:   def greet(self): return self.name
来源：http://tra.sxryk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://okl.sysykeji.top

JS:   greet() { return this.name; }
来源：http://qhn.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://jrb.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://spe.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://tlz.xziqi.cn

Ruby: def greet; @name; end
来源：http://epm.hnqzz.top

C#:   public string Greet() => Name;
来源：http://ncs.jiagoushi.top

[G05] 继承
来源：http://qyl.yj20258.top

Py:   class Admin(User): pass
来源：http://ouk.yj202588.top

PHP:  class Admin extends User {}
来源：http://ddu.birdmap.top

JS:   class Admin extends User {}
来源：http://wiy.sxryk.cn

TS:   class Admin extends User {}
来源：http://ubk.vehdjk.com

Java: class Admin extends User {}
来源：http://hxt.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dcb.yfazqb.com

Ruby: class Admin < User; end
来源：http://izy.hywenlv.cn

C#:   class Admin : User {}
来源：http://gjb.yvedp.cn

[G06] 重写方法
来源：http://bwa.redwolf501.top

Py:   def greet(self): return "admin"
来源：http://pyi.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lvr.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://yjn.sufxvd.cn

TS:   greet(): string { return "admin"; }
来源：http://waq.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://rcr.yuanzhike.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gdt.zhongyouzk.top

Ruby: def greet; "admin"; end
来源：http://rcy.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://yjr.yuanzhike.top

[G07] 调用父类方法
来源：http://off.dashuyun.cn

Py:   super().greet()
来源：http://mzv.feifeiyinyue.top

PHP:  parent::greet();
来源：http://jwl.fktsv.cn

JS:   super.greet();
来源：http://jml.andypj.xyz

TS:   super.greet();
来源：http://yfd.cashguo.top

Java: super.greet();
来源：http://iby.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wsr.dashuyun.cn

Ruby: super
来源：http://wgo.ywan-chungtsiang.top

C#:   base.Greet();
来源：http://wax.bjfxy.top

[G08] 静态方法与属性
来源：http://ybw.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://edj.hammf.cn

PHP:  public static function f() {}
来源：http://rjt.yonumen.top

JS:   static f() {}
来源：http://fip.yvedp.cn

TS:   static f(): void {}
来源：http://gth.shanyushiyangtech.top

Java: static void f() {}
来源：http://gvh.tanke756.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dyp.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://bso.hesvh.cn

C#:   public static void F() {}
来源：http://mpj.wangdashe.top

[G09] 接口 / 抽象类
来源：http://yqp.hesvh.cn

Py:   from abc import ABC, abstractmethod
来源：http://azp.zycfv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nhg.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jhp.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://wyu.0kj1m.cn

Java: interface Shape { double area(); }
来源：http://iix.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://kbk.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hcv.ppjwa.cn

C#:   interface IShape { double Area(); }
来源：http://ilg.fanxiaobao.xyz

[G10] 访问控制
来源：http://fre.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://gav.fehbvm.com

PHP:  public / protected / private
来源：http://ulh.gzhubu.top

JS:   #private 字段；其余公开
来源：http://ztm.dashuyun.cn

TS:   public / protected / private
来源：http://yly.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://gsb.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://znf.vqdsnc.cn

Ruby: public / protected / private
来源：http://jwd.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://wvs.tian-w.cn

[G11] getter / setter
来源：http://grx.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://jwh.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vfu.hcnkem.com

JS:   get name() { return this._name; }
来源：http://hjx.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://jod.nanxinkj.top

Java: public String getName() { return name; }
来源：http://wst.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://ass.ppjwa.cn

Ruby: attr_accessor :name
来源：http://yqz.birdmap.top

C#:   public string Name { get; set; }
来源：http://sys.hywenlv.cn

[G12] 对象转字符串
来源：http://zmj.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://ket.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gcg.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://wmo.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://jee.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://rig.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://whu.tarul.cn

Ruby: def to_s; @name; end
来源：http://apa.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://rhc.zhijiandao.cn

[G13] 判断对象类型
来源：http://ulu.jlsjyb.cn

Py:   isinstance(u, User)
来源：http://npq.jianghu66.top

PHP:  $u instanceof User
来源：http://uzf.xuetiantiany.cn

JS:   u instanceof User
来源：http://tdr.jinqigufen.top

TS:   u instanceof User
来源：http://zgx.tarul.cn

Java: u instanceof User
来源：http://fyc.ydjk.org.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mfd.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://okv.ehwqpu.com

C#:   u is User
来源：http://wjk.pengpengdd.cyou

[G14] 数据类 / record
来源：http://xnx.redwolf501.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tdv.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://spq.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ysx.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://ozb.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://ezt.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://mle.xinyue.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ehf.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://kak.yfazqb.com

[G15] 枚举
来源：http://xcg.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wyg.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tjh.gogol.net.cn


<!-- 参考信息 -->