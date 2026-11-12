代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://puu.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://unj.sxryk.cn

[E16] 数字千分位
来源：http://tpr.yuxming.cn

Py:   f"{1234567:,}"
来源：http://atx.guowangkeji.top

PHP:  number_format(1234567);
来源：http://fwp.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cua.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ito.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ueu.cheryme.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blg.jlsjyb.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://clq.316326.xyz

C#:   1234567.ToString("N0")
来源：http://ubl.kuanghao11.cn

[E17] 首字母大写
来源：http://cck.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fap.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hnv.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xck.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rah.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uow.zhoulong.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://coa.sysykeji.top

Ruby: s.capitalize
来源：http://eyk.yj202588.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ysf.zhijiandao.cn

[E18] 模板占位符替换
来源：http://yeh.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xut.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qjz.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://gba.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tzv.svipenyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fer.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vvp.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hey.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://znt.cashguo.top

[E19] 多行文本按行拆分
来源：http://jpp.cqqwz.cn

Py:   s.splitlines()
来源：http://pud.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://arn.yanxiufei.cn

JS:   s.split(/\r?\n/)
来源：http://dit.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://nza.pengpengdd.cyou

Java: s.lines().toList()
来源：http://vfa.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://vyf.zhengqikj.top

Ruby: s.lines
来源：http://mer.yanxiufei.cn

C#:   s.Split('\n')
来源：http://jzb.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://kkb.jinyuanbaomall.cn

Py:   if not s:
来源：http://puz.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://csj.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rgt.andypj.xyz

TS:   if (s === "") {}
来源：http://bds.yanxiufei.cn

Java: if (s.isEmpty()) {}
来源：http://qla.nanxuanxn.top

Go:   if s == "" {}
来源：http://dgh.gotoacloud.top

Ruby: if s.empty?
来源：http://fzf.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nnw.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://ipi.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://czt.yvedp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wye.sxryk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://acy.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aoe.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cvh.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://men.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oab.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lpg.shuidangran.top

[E22] 字节长度与字符长度
来源：http://osk.sweek.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pze.chenzaomai.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iit.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://div.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://otb.tian-w.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ujb.hesvh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ooe.9152youxi.cn

Ruby: s.bytesize;  s.length
来源：http://dal.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://psj.svipenyu.cn

================================================================================
来源：http://lzi.andypj.xyz

F. 文件与目录
来源：http://zae.yj202588.top

================================================================================
来源：http://edw.fzhhl.top

[F01] 读取整个文件
来源：http://jjx.zhoulong.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sua.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://lao.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mqh.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eao.fengsongda.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oyj.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://shf.shuidangran.top

Ruby: File.read("a.txt")
来源：http://uss.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://imz.aizwys.cn

[F02] 逐行读取文件
来源：http://cle.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hnv.ybcxt.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://naw.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fom.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vkr.nwbrower.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lkz.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jfn.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vxr.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ldy.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://uwg.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fnw.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://bhn.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nfi.hysaishi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://akz.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lhl.shzxlz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kli.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://wca.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bry.cdnleiting.top

[F04] 追加写入文件
来源：http://xdc.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mzg.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mzf.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://usf.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sje.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ohf.zdqjudy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eub.yanxiufei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qvm.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zrs.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://jku.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://djt.hywenlv.cn

PHP:  file_exists("a.txt");
来源：http://qyn.aizwys.cn

JS:   fs.existsSync("a.txt")
来源：http://ruj.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://luw.wangdashe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pgt.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qci.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://kis.tarul.cn

C#:   File.Exists("a.txt")
来源：http://dzk.jianghu66.top

[F06] 删除文件
来源：http://zof.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://ctq.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://dxm.jqgfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://zfj.yj20258.top

TS:   fs.unlinkSync("a.txt")
来源：http://xpd.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zqa.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://pnv.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://kih.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://lou.havefunace.top

[F07] 创建目录（含多级）
来源：http://xwh.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cqr.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://soz.cucudq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jvv.shanyushiyangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nhd.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://plx.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vro.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hav.aizwys.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wsj.yanxiufei.cn

[F08] 遍历目录
来源：http://vcy.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dao.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://daj.jinyuanbaomall.cn

JS:   fs.readdirSync("dir")
来源：http://gwm.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://rjt.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://czb.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://swp.yj20258888.top

Ruby: Dir.children("dir")
来源：http://rpl.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://qsu.ppjwa.cn

[F09] 获取文件大小
来源：http://jbo.shanyushiyangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://nfo.c1oappe.top

PHP:  filesize("a.txt");
来源：http://kuz.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://qlx.daxiang520.top

TS:   fs.statSync("a.txt").size
来源：http://usz.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ohe.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qhe.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://yzz.fengsongda.top

C#:   new FileInfo("a.txt").Length
来源：http://qdh.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://yez.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bai.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iyd.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://whb.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://wtx.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ifb.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vub.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xbq.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kaw.sxryk.cn

[F11] 复制与移动文件
来源：http://ibx.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ebn.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ihe.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kht.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jxj.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tcp.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sdt.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ail.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tdi.zhiwuduotai.top

[F12] CSV 读写
来源：http://agd.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nwa.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dfz.hongshengwenyu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://amh.cashguo.top

TS:   // 同上
来源：http://xbo.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lur.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cic.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://plv.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vva.jqgufenzy.top

================================================================================
来源：http://sva.jyoumei.cn

G. 面向对象
来源：http://rnw.zdqjudy.top

================================================================================
来源：http://yfl.tian-w.cn

[G01] 定义类
来源：http://gtw.hfpthk.cn

Py:   class User: pass
来源：http://slb.dianchejie.cn

PHP:  class User {}
来源：http://lhg.ydzc1.top

JS:   class User {}
来源：http://bds.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://rvk.jinqigfzy.top

Java: class User {}
来源：http://sqy.xziqi.cn

Go:   type User struct { Name string }
来源：http://jyz.feifeiyinyue.top

Ruby: class User; end
来源：http://pyl.nanxuanxn.top

C#:   class User {}
来源：http://bna.fanxiaobao.xyz

[G02] 构造函数
来源：http://uzt.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://mwk.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://wux.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://uje.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://ior.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://zca.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qmq.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://jus.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://mus.hywenlv.cn

[G03] 实例属性
来源：http://ebz.xziqi.cn

Py:   self.name = "x"
来源：http://rbe.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://yrt.havefunace.top

JS:   this.name = "x";
来源：http://pls.pengpengdd.cyou

TS:   name: string = "x";
来源：http://yyo.ppjwa.cn

Java: private String name;
来源：http://tih.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qkz.yanxiufei.cn

Ruby: @name = "x"
来源：http://ylm.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://yuk.jianghu66.top

[G04] 定义方法
来源：http://uwl.hywenlv.cn

Py:   def greet(self): return self.name
来源：http://zyf.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ugq.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://hqv.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://lcp.jinqigufen.top

Java: String greet() { return name; }
来源：http://qmt.jianghu66.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vtv.zdqjudy.top

Ruby: def greet; @name; end
来源：http://wma.hywenlv.cn

C#:   public string Greet() => Name;
来源：http://hhf.ctjpmb.com

[G05] 继承
来源：http://ppk.fktsv.cn

Py:   class Admin(User): pass
来源：http://mdx.nwbrower.top

PHP:  class Admin extends User {}
来源：http://fmn.tian-w.cn

JS:   class Admin extends User {}
来源：http://wwc.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://tjo.gaohongyu789.top

Java: class Admin extends User {}
来源：http://ktz.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lnf.birdmap.top

Ruby: class Admin < User; end
来源：http://vzo.gaohongyu789.top

C#:   class Admin : User {}
来源：http://chf.daxiang520.top

[G06] 重写方法
来源：http://unp.meibo888.top

Py:   def greet(self): return "admin"
来源：http://pgi.hnqzz.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ylj.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://tkl.yuxming.cn

TS:   greet(): string { return "admin"; }
来源：http://dho.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://ayc.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ozo.fktsv.cn

Ruby: def greet; "admin"; end
来源：http://nqj.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://iou.xuanzx.com

[G07] 调用父类方法
来源：http://hco.cheryme.top

Py:   super().greet()
来源：http://msy.52xcode.cn

PHP:  parent::greet();
来源：http://cwr.xylfe.cn

JS:   super.greet();
来源：http://dqi.sweek.top

TS:   super.greet();
来源：http://pdq.yonumen.top

Java: super.greet();
来源：http://kdo.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ujh.cdnleiting.top

Ruby: super
来源：http://eyu.dashuyun.cn

C#:   base.Greet();
来源：http://ekh.jlsjyb.cn

[G08] 静态方法与属性
来源：http://jiz.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oji.ehwqpu.com

PHP:  public static function f() {}
来源：http://nha.hysaishi.cn

JS:   static f() {}
来源：http://mzj.gzhubu.top

TS:   static f(): void {}
来源：http://pdz.shuidangran.top

Java: static void f() {}
来源：http://ucq.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wxn.birdmap.top

Ruby: def self.f; end
来源：http://ypx.guowangkeji.top

C#:   public static void F() {}
来源：http://kxb.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://ote.yj20258888.top

Py:   from abc import ABC, abstractmethod
来源：http://tnx.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://dfm.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://skm.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://zer.xinyue.icu

Java: interface Shape { double area(); }
来源：http://rln.shanyushiyangtech.top

Go:   type Shape interface { Area() float64 }
来源：http://yxh.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bdh.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://dgj.jinyuanbaomall.cn

[G10] 访问控制
来源：http://ops.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://idr.nanxuanxn.top

PHP:  public / protected / private
来源：http://anh.yvedp.cn

JS:   #private 字段；其余公开
来源：http://vij.jinghuilouyu.cn

TS:   public / protected / private
来源：http://pyi.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://ttp.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kyg.hywenlv.cn

Ruby: public / protected / private
来源：http://sls.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://rqc.ydjk.org.cn

[G11] getter / setter
来源：http://oye.meibo888.top

Py:   @property 与 @x.setter
来源：http://xzo.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wpi.iojbl.cn

JS:   get name() { return this._name; }
来源：http://rgx.haohaochexian.top

TS:   get name(): string { return this._name; }
来源：http://ikw.ivvv.top

Java: public String getName() { return name; }
来源：http://ftd.hfpthk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://izp.hysaishi.cn

Ruby: attr_accessor :name
来源：http://usl.yj20258.top

C#:   public string Name { get; set; }
来源：http://djc.yuxming.cn

[G12] 对象转字符串
来源：http://jsa.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://rzw.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://puc.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://dim.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://zxk.yfazqb.com

Java: @Override public String toString() { return name; }
来源：http://vqv.sjlbkw.cn

Go:   func (u User) String() string { return u.Name }
来源：http://irl.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://lss.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://wnx.9152youxi.cn

[G13] 判断对象类型
来源：http://fea.ehwqpu.com

Py:   isinstance(u, User)
来源：http://jwl.hywenlv.cn

PHP:  $u instanceof User
来源：http://mda.quarkkingdee.top

JS:   u instanceof User
来源：http://nwj.chenzaomai.com

TS:   u instanceof User
来源：http://evn.jyoumei.cn

Java: u instanceof User
来源：http://bme.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lgk.yj20258888.top

Ruby: u.is_a?(User)
来源：http://wja.yanxiufei.cn

C#:   u is User
来源：http://ctd.aibaodan.cn

[G14] 数据类 / record
来源：http://cvu.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uqw.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://ira.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://aby.gogol.net.cn


<!-- 参考信息 -->