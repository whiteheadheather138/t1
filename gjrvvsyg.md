代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yrc.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jag.yueranfly.top

[E16] 数字千分位
来源：http://gml.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://wfb.guowangkeji.top

PHP:  number_format(1234567);
来源：http://rrw.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://npf.cqqwz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mzr.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bmr.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rpl.chenzaomai.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://auy.yj20258.top

C#:   1234567.ToString("N0")
来源：http://ctt.ybcxt.top

[E17] 首字母大写
来源：http://vzu.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tyy.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://bha.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bym.gaohongyu789.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://toe.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zjp.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ubb.xziqi.cn

Ruby: s.capitalize
来源：http://yuk.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bcv.yfazqb.com

[E18] 模板占位符替换
来源：http://lot.chenjidiqi.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vxi.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ywu.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://xsu.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mvm.sysykeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vec.cashguo.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://glo.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vhx.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xck.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://iii.gzhubu.top

Py:   s.splitlines()
来源：http://nlh.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://evq.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://aag.iojbl.cn

TS:   s.split(/\r?\n/)
来源：http://zdl.fengsongda.top

Java: s.lines().toList()
来源：http://pby.uphjek.com

Go:   strings.Split(s, "\n")
来源：http://pno.kuanghao11.cn

Ruby: s.lines
来源：http://cbq.0kj1m.cn

C#:   s.Split('\n')
来源：http://hiq.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://jqg.nanxuanxn.top

Py:   if not s:
来源：http://mhl.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ybl.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eiu.hammf.cn

TS:   if (s === "") {}
来源：http://kyo.0kj1m.cn

Java: if (s.isEmpty()) {}
来源：http://gso.ydzc1.top

Go:   if s == "" {}
来源：http://nkd.haohaochexian.top

Ruby: if s.empty?
来源：http://yrs.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zgf.daria6918.cn

[E21] 超长截断加省略号
来源：http://pzf.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nal.zycfv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mrf.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jin.xuetiantiany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zuk.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qtd.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://eaw.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eqc.c1oappe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://osz.ehwqpu.com

[E22] 字节长度与字符长度
来源：http://wpz.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ubz.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hwt.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nle.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qrf.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://srw.316326.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ghw.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://hwz.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xpf.tianlin.xyz

================================================================================
来源：http://ewg.svipenyu.cn

F. 文件与目录
来源：http://oia.iojbl.cn

================================================================================
来源：http://gmf.yongpay.top

[F01] 读取整个文件
来源：http://qxx.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mey.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://rrv.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zoi.zhaomingkeji.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pbh.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fon.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://npc.yanxiufei.cn

Ruby: File.read("a.txt")
来源：http://khp.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://cxv.ybcxt.top

[F02] 逐行读取文件
来源：http://uez.xinyue.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wws.xuetiantiany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rsx.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ouk.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bbv.gogol.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://und.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qsw.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://auj.guannengcc.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fqb.sjlbkw.cn

[F03] 写入文件（覆盖）
来源：http://dvk.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://acq.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nnc.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dtw.shzxlz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jfr.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wso.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rhi.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://duh.cheryme.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dej.hammf.cn

[F04] 追加写入文件
来源：http://vjk.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ndb.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gbj.yj20258888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wgg.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oca.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cwt.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xyj.yuanzhike.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://icy.fanxiaobao.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tku.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://qth.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://djk.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://jyq.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://tup.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://lhi.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hxn.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ytu.ppjwa.cn

Ruby: File.exist?("a.txt")
来源：http://wtm.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://zyq.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://oiz.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://rbk.bbcook.cn

PHP:  unlink("a.txt");
来源：http://aqe.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://zcq.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://szg.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qlm.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://oei.gotoacloud.top

Ruby: File.delete("a.txt")
来源：http://sft.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://myl.cqqwz.cn

[F07] 创建目录（含多级）
来源：http://aqo.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cuw.sysykeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kyr.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tla.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fqd.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dxn.yuxming.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mim.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vac.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nhk.ppjwa.cn

[F08] 遍历目录
来源：http://cmr.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://btn.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aoz.vqdsnc.cn

JS:   fs.readdirSync("dir")
来源：http://uaj.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://eus.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gyx.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rud.vehdjk.com

Ruby: Dir.children("dir")
来源：http://gim.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://cnw.yangfankeji.com

[F09] 获取文件大小
来源：http://heu.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://voh.c1oappe.top

PHP:  filesize("a.txt");
来源：http://bhc.xingfuxueyuan.xyz

JS:   fs.statSync("a.txt").size
来源：http://ohn.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://lue.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rxo.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ibh.hongshengwenyu.top

Ruby: File.size("a.txt")
来源：http://ciw.xuetiantiany.cn

C#:   new FileInfo("a.txt").Length
来源：http://zgi.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://ygk.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jii.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tvo.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pea.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://nhr.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xvn.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bup.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vlj.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lgh.0kj1m.cn

[F11] 复制与移动文件
来源：http://ecr.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gcb.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://unq.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fcb.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hph.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://klg.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tsj.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lhe.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://txs.dianchejie.cn

[F12] CSV 读写
来源：http://vxz.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lei.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hxx.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bwb.jiagoushi.top

TS:   // 同上
来源：http://rrh.wangshuangyany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://thj.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bxn.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zlm.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dwz.fktsv.cn

================================================================================
来源：http://lvc.sysykeji.top

G. 面向对象
来源：http://cff.hywenlv.cn

================================================================================
来源：http://gco.zdqjudy.top

[G01] 定义类
来源：http://ean.xuanzx.com

Py:   class User: pass
来源：http://otr.guannengcc.top

PHP:  class User {}
来源：http://qbp.sweek.top

JS:   class User {}
来源：http://mlj.haohaochexian.top

TS:   class User { name: string = ""; }
来源：http://pnz.dianchejie.cn

Java: class User {}
来源：http://qol.hammf.cn

Go:   type User struct { Name string }
来源：http://aot.cucudq.cn

Ruby: class User; end
来源：http://bdq.yuxming.cn

C#:   class User {}
来源：http://qhb.yuanzhike.top

[G02] 构造函数
来源：http://yir.shangyingyoupin.top

Py:   def __init__(self, name): self.name = name
来源：http://fla.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://zzc.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://dbj.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://ryf.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://lgh.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bba.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://gun.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://bjz.sufxvd.cn

[G03] 实例属性
来源：http://ayb.shzxlz.cn

Py:   self.name = "x"
来源：http://ixz.aizwys.cn

PHP:  public string $name = "x";
来源：http://vru.aibaodan.cn

JS:   this.name = "x";
来源：http://jxp.gzhubu.top

TS:   name: string = "x";
来源：http://zui.feifeiyinyue.top

Java: private String name;
来源：http://zlk.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tev.kuanghao11.cn

Ruby: @name = "x"
来源：http://krz.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://ioa.birdmap.top

[G04] 定义方法
来源：http://tym.zycfv.cn

Py:   def greet(self): return self.name
来源：http://bqu.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://shm.cashguo.top

JS:   greet() { return this.name; }
来源：http://mqj.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://aml.gotoacloud.top

Java: String greet() { return name; }
来源：http://egd.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ucv.hesvh.cn

Ruby: def greet; @name; end
来源：http://wja.wangdashe.top

C#:   public string Greet() => Name;
来源：http://pbu.uphjek.com

[G05] 继承
来源：http://hdj.xingfuxueyuan.xyz

Py:   class Admin(User): pass
来源：http://rdw.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://ajt.dianchejie.cn

JS:   class Admin extends User {}
来源：http://gqw.316326.xyz

TS:   class Admin extends User {}
来源：http://qsu.hywenlv.cn

Java: class Admin extends User {}
来源：http://mun.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nxf.yj202588.top

Ruby: class Admin < User; end
来源：http://tfj.ctjpmb.com

C#:   class Admin : User {}
来源：http://ryz.yuanzhike.top

[G06] 重写方法
来源：http://asr.shangyingyoupin.top

Py:   def greet(self): return "admin"
来源：http://gke.nwbrower.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pla.sweek.top

JS:   greet() { return "admin"; }
来源：http://eyi.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://ouw.zhixingplan.top

Java: @Override String greet() { return "admin"; }
来源：http://flk.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oll.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://ezg.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://ipg.yfazqb.com

[G07] 调用父类方法
来源：http://qlb.aizwys.cn

Py:   super().greet()
来源：http://cqu.aibaodan.cn

PHP:  parent::greet();
来源：http://uut.jqgfzy.top

JS:   super.greet();
来源：http://rrk.wangshuangyany.cn

TS:   super.greet();
来源：http://iyv.shangyingyoupin.top

Java: super.greet();
来源：http://xoc.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zqo.wangshuangyany.cn

Ruby: super
来源：http://hbj.jyoumei.cn

C#:   base.Greet();
来源：http://ctq.cheryme.top

[G08] 静态方法与属性
来源：http://sgp.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://efd.shzxlz.cn

PHP:  public static function f() {}
来源：http://kfp.gzhubu.top

JS:   static f() {}
来源：http://yfg.ivvv.top

TS:   static f(): void {}
来源：http://jyb.smart0.xyz

Java: static void f() {}
来源：http://jnr.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ewa.pycfn.com

Ruby: def self.f; end
来源：http://hgo.tianlin.xyz

C#:   public static void F() {}
来源：http://otj.mhx1999.top

[G09] 接口 / 抽象类
来源：http://eeb.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://uzo.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bdf.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ubb.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://gzr.ybcxt.top

Java: interface Shape { double area(); }
来源：http://ynt.guannengcc.top

Go:   type Shape interface { Area() float64 }
来源：http://cwi.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iqm.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://nrn.chenzaomai.com

[G10] 访问控制
来源：http://uuy.guannengcc.top

Py:   约定 _protected / __private（不强制）
来源：http://mnu.c1oappe.top

PHP:  public / protected / private
来源：http://rmw.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://fbq.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://tqd.sweek.top

Java: public / protected / private / 默认包级
来源：http://wzo.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ylg.feifeiyinyue.top

Ruby: public / protected / private
来源：http://efb.zhijiandao.cn

C#:   public / protected / private / internal
来源：http://rrp.aibaodan.cn

[G11] getter / setter
来源：http://nsu.fanxiaobao.xyz

Py:   @property 与 @x.setter
来源：http://xdf.hfpthk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vit.dashuyun.cn

JS:   get name() { return this._name; }
来源：http://gzh.nanxinkj.top

TS:   get name(): string { return this._name; }
来源：http://ltj.jqgfzy.top

Java: public String getName() { return name; }
来源：http://grg.vqdsnc.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://esa.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://jkr.vehdjk.com

C#:   public string Name { get; set; }
来源：http://jey.ivvv.top

[G12] 对象转字符串
来源：http://oaj.feifeiyinyue.top

Py:   def __str__(self): return self.name
来源：http://zuk.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fuu.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://luj.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://nfh.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://lba.yuxming.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wmc.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://cwf.pycfn.com

C#:   public override string ToString() => Name;
来源：http://abq.zycfv.cn

[G13] 判断对象类型
来源：http://jph.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://gpa.gotoacloud.top

PHP:  $u instanceof User
来源：http://ecx.redwolf501.top

JS:   u instanceof User
来源：http://ghb.pycfn.com

TS:   u instanceof User
来源：http://pxs.gotoacloud.top

Java: u instanceof User
来源：http://mxr.shuidangran.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oxh.yvedp.cn

Ruby: u.is_a?(User)
来源：http://rpf.zhoulong.xyz

C#:   u is User
来源：http://bzo.ppjwa.cn

[G14] 数据类 / record
来源：http://nxl.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gfe.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://ixp.hfpthk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bcr.andypj.xyz


<!-- 参考信息 -->