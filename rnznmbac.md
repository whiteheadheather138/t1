代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fft.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cfg.gotoacloud.top

[E16] 数字千分位
来源：http://jcx.wangdashe.top

Py:   f"{1234567:,}"
来源：http://can.fehbvm.com

PHP:  number_format(1234567);
来源：http://pmf.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tqg.shuidangran.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qpa.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ghv.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zfv.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jag.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://mvb.jiagoushi.top

[E17] 首字母大写
来源：http://ykp.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://glw.ivvv.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yyo.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tbr.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tnm.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ewg.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nip.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://alb.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lcj.c1oappe.top

[E18] 模板占位符替换
来源：http://eyy.bbcook.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://trt.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jbn.jinqigfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ema.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://ajw.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tzf.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://brq.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mym.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gum.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://juh.zhoulong.xyz

Py:   s.splitlines()
来源：http://gva.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wst.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://owl.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://iqz.daxiang520.top

Java: s.lines().toList()
来源：http://bcb.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://rao.zhijiandao.cn

Ruby: s.lines
来源：http://ufv.hywenlv.cn

C#:   s.Split('\n')
来源：http://hui.hnqzz.top

[E20] 判断字符串是否为空
来源：http://euf.yj20258888.top

Py:   if not s:
来源：http://qyi.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ssi.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mzh.sjlbkw.cn

TS:   if (s === "") {}
来源：http://him.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://bft.hnxiangtu.top

Go:   if s == "" {}
来源：http://iiq.yueranfly.top

Ruby: if s.empty?
来源：http://vsv.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mmn.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://ffw.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kkg.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ivn.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gbn.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uvh.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jcn.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://qhh.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bnr.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xez.hammf.cn

[E22] 字节长度与字符长度
来源：http://iig.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://abq.sysykeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sqt.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xrh.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yrm.zhiwuduotai.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://geb.hesvh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mhp.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://nwz.pengpengdd.cyou

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cbp.nanxinkj.top

================================================================================
来源：http://aaa.svipenyu.cn

F. 文件与目录
来源：http://ctc.vehdjk.com

================================================================================
来源：http://uuh.hnqzz.top

[F01] 读取整个文件
来源：http://wlu.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vuu.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://lgi.hfpthk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tje.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://myo.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ltf.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dsh.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://ptk.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://mcj.dashuyun.cn

[F02] 逐行读取文件
来源：http://upo.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aiz.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://toy.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wbb.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gnr.nwbrower.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jpm.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aak.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jka.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tev.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://can.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cir.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zla.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qkc.ppjwa.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jhw.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yfv.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nzl.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://szl.birdmap.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://soc.hysaishi.cn

[F04] 追加写入文件
来源：http://wug.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nfk.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rhc.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://spk.xingfuxueyuan.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://klv.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oki.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://txs.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wec.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qqf.jinghuilouyu.cn

[F05] 判断文件或目录是否存在
来源：http://baf.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mou.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://jnc.fktsv.cn

JS:   fs.existsSync("a.txt")
来源：http://sre.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://uit.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yiv.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vdr.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://dwg.daxiang520.top

C#:   File.Exists("a.txt")
来源：http://mra.shangyingyoupin.top

[F06] 删除文件
来源：http://xdu.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://zsa.xinyue.icu

PHP:  unlink("a.txt");
来源：http://bdx.daria6918.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pqs.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://uqg.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ikc.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://mfj.uphjek.com

Ruby: File.delete("a.txt")
来源：http://gxx.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://qin.hesvh.cn

[F07] 创建目录（含多级）
来源：http://ilr.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kik.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://exf.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dje.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://edd.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://csp.jyoumei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jck.xuanzx.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://skf.sufxvd.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://smt.shanyushiyangtech.top

[F08] 遍历目录
来源：http://zoj.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zhj.yuxming.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://alq.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://jer.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://xvk.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tzg.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://ycw.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://riy.aizwys.cn

C#:   Directory.GetFiles("dir")
来源：http://xbi.uphjek.com

[F09] 获取文件大小
来源：http://zmh.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://cjf.gzhubu.top

PHP:  filesize("a.txt");
来源：http://gcr.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://ibb.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://ekx.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://itx.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pmj.52xcode.cn

Ruby: File.size("a.txt")
来源：http://unc.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://yfo.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://ywz.shzxlz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rch.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tfg.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uaa.hesvh.cn

TS:   path.extname("a.txt")
来源：http://yoy.hnqzz.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://guo.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dou.vehdjk.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://opx.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hdt.snrcjt.cn

[F11] 复制与移动文件
来源：http://omt.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qsh.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mru.bjfxy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://usl.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dox.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pjh.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ecs.xingfuxueyuan.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ygy.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jgg.jqgufenzy.top

[F12] CSV 读写
来源：http://duh.nwbrower.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mev.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dds.tianlin.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fad.nanxuanxn.top

TS:   // 同上
来源：http://okf.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ref.smart0.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iuj.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ddy.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rrd.hesvh.cn

================================================================================
来源：http://oik.yj20258.top

G. 面向对象
来源：http://yeg.yfazqb.com

================================================================================
来源：http://kez.yuxming.cn

[G01] 定义类
来源：http://ogw.ydzc1.top

Py:   class User: pass
来源：http://fkc.gotoacloud.top

PHP:  class User {}
来源：http://qfo.kuanghao11.cn

JS:   class User {}
来源：http://nqw.52xcode.cn

TS:   class User { name: string = ""; }
来源：http://bku.zhijiandao.cn

Java: class User {}
来源：http://vbh.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://qht.jianghu66.top

Ruby: class User; end
来源：http://eyx.xingfuxueyuan.xyz

C#:   class User {}
来源：http://rgb.hfpthk.cn

[G02] 构造函数
来源：http://niu.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://mae.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://egh.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://xkn.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://qej.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://yna.yvedp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mxv.fengsongda.top

Ruby: def initialize(name); @name = name; end
来源：http://fzx.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://mhj.sysykeji.top

[G03] 实例属性
来源：http://wph.tian-w.cn

Py:   self.name = "x"
来源：http://hpg.meibo888.top

PHP:  public string $name = "x";
来源：http://deu.ehwqpu.com

JS:   this.name = "x";
来源：http://rvv.sweek.top

TS:   name: string = "x";
来源：http://lmj.fengsongda.top

Java: private String name;
来源：http://ipx.jinyuanbaomall.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jtb.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://dsc.chenlongwang.top

C#:   public string Name { get; set; } = "x";
来源：http://zle.haohaochexian.top

[G04] 定义方法
来源：http://gmp.chenjidiqi.icu

Py:   def greet(self): return self.name
来源：http://juh.wangdashe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ygc.jianghu66.top

JS:   greet() { return this.name; }
来源：http://tii.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://pod.sxryk.cn

Java: String greet() { return name; }
来源：http://fmm.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pbm.quarkkingdee.top

Ruby: def greet; @name; end
来源：http://lfv.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://mfn.feifeiyinyue.top

[G05] 继承
来源：http://qfm.zycfv.cn

Py:   class Admin(User): pass
来源：http://srj.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://isz.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://ucp.hywenlv.cn

TS:   class Admin extends User {}
来源：http://fen.quarkkingdee.top

Java: class Admin extends User {}
来源：http://zoj.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lek.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://tri.jlsjyb.cn

C#:   class Admin : User {}
来源：http://bju.bbcook.cn

[G06] 重写方法
来源：http://brr.hywenlv.cn

Py:   def greet(self): return "admin"
来源：http://ilm.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vzd.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://sen.jianghu66.top

TS:   greet(): string { return "admin"; }
来源：http://aod.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://gol.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mgd.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://zcv.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://efs.jinqigfzy.top

[G07] 调用父类方法
来源：http://ycm.wangdashe.top

Py:   super().greet()
来源：http://ndh.wangdashe.top

PHP:  parent::greet();
来源：http://low.kuanghao11.cn

JS:   super.greet();
来源：http://jge.yj20258.top

TS:   super.greet();
来源：http://grg.ppjwa.cn

Java: super.greet();
来源：http://nsm.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ddj.shzxlz.cn

Ruby: super
来源：http://jmx.zycfv.cn

C#:   base.Greet();
来源：http://gbl.zhengqikj.top

[G08] 静态方法与属性
来源：http://bue.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hfo.yj20258888.top

PHP:  public static function f() {}
来源：http://zeg.uphjek.com

JS:   static f() {}
来源：http://dft.yj20258888.top

TS:   static f(): void {}
来源：http://ytv.yueranfly.top

Java: static void f() {}
来源：http://xyo.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cfu.xinyue.icu

Ruby: def self.f; end
来源：http://mwf.shzxlz.cn

C#:   public static void F() {}
来源：http://xrd.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://bur.xuanzx.com

Py:   from abc import ABC, abstractmethod
来源：http://yyj.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cft.hywenlv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ioz.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://lsx.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://vdq.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://nml.zdqjudy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eim.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://ayk.chenlongwang.top

[G10] 访问控制
来源：http://lca.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://otj.tanke756.top

PHP:  public / protected / private
来源：http://vkb.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://oqz.bbcook.cn

TS:   public / protected / private
来源：http://tla.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://olm.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cho.yuanzhike.top

Ruby: public / protected / private
来源：http://aty.meibo888.top

C#:   public / protected / private / internal
来源：http://bgc.tian-w.cn

[G11] getter / setter
来源：http://ebi.wangdashe.top

Py:   @property 与 @x.setter
来源：http://qzk.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jwe.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://puj.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://ehu.sysykeji.top

Java: public String getName() { return name; }
来源：http://jyh.9152youxi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wsc.cheryme.top

Ruby: attr_accessor :name
来源：http://xsz.andypj.xyz

C#:   public string Name { get; set; }
来源：http://cyp.ydjk.org.cn

[G12] 对象转字符串
来源：http://ddw.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://vhm.jqgfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rta.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://bwm.sweek.top

TS:   toString(): string { return this.name; }
来源：http://oug.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://myo.sysykeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://hkj.yanxiufei.cn

Ruby: def to_s; @name; end
来源：http://usk.jqgufenzy.top

C#:   public override string ToString() => Name;
来源：http://rpy.jianghu66.top

[G13] 判断对象类型
来源：http://gwm.sufxvd.cn

Py:   isinstance(u, User)
来源：http://ocz.bbcook.cn

PHP:  $u instanceof User
来源：http://qcr.nanxuanxn.top

JS:   u instanceof User
来源：http://dsd.ppjwa.cn

TS:   u instanceof User
来源：http://uhc.ydjk.org.cn

Java: u instanceof User
来源：http://nfj.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://wko.hnqzz.top

Ruby: u.is_a?(User)
来源：http://mmu.birdmap.top

C#:   u is User
来源：http://wmw.jyoumei.cn

[G14] 数据类 / record
来源：http://jxu.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://itl.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://qll.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://kld.52xcode.cn


<!-- 参考信息 -->