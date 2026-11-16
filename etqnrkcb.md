代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://apg.ydjk.org.cn

[E15] HTML 转义 / 反转义
来源：http://nkb.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nvn.zycfv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zeb.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jyb.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rln.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pvu.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fdh.redwolf501.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yxn.haohaochexian.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gbp.yueranfly.top

[E16] 数字千分位
来源：http://bsk.yueranfly.top

Py:   f"{1234567:,}"
来源：http://qmq.uphjek.com

PHP:  number_format(1234567);
来源：http://knu.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jun.gogol.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dib.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mqt.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dkr.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://txc.xingfuxueyuan.xyz

C#:   1234567.ToString("N0")
来源：http://uzl.yuxming.cn

[E17] 首字母大写
来源：http://vrs.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iuo.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dle.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hln.yuxming.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://swz.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ngc.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fjb.0kj1m.cn

Ruby: s.capitalize
来源：http://dva.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mnp.wangdashe.top

[E18] 模板占位符替换
来源：http://rcz.vqdsnc.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iyw.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ocz.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xsk.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://srw.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kjv.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vmt.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fnk.yuanzhike.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ich.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://flu.guowangkeji.top

Py:   s.splitlines()
来源：http://vdn.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mjq.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://eey.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://fve.vehdjk.com

Java: s.lines().toList()
来源：http://lbf.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://xay.cucudq.cn

Ruby: s.lines
来源：http://xqq.yangfankeji.com

C#:   s.Split('\n')
来源：http://zpf.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://ipf.birdmap.top

Py:   if not s:
来源：http://ref.epnwcf.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uco.zdqjudy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ste.guannengcc.top

TS:   if (s === "") {}
来源：http://qhu.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://pnx.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://koq.kuanghao11.cn

Ruby: if s.empty?
来源：http://uyw.zdqjudy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rap.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://hbj.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ofp.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://utv.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lgu.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fkf.nanxuanxn.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ayk.52xcode.cn

Go:   // 按 rune 判断长度后截断
来源：http://mkk.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ozj.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://utp.yueranfly.top

[E22] 字节长度与字符长度
来源：http://ubx.jlsjyb.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mgo.andypj.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iey.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://orn.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wmw.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tjs.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xcj.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://yhl.jqgfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://duj.gotoacloud.top

================================================================================
来源：http://mej.yanxiufei.cn

F. 文件与目录
来源：http://vwo.yj202588.top

================================================================================
来源：http://uol.jinqigfzy.top

[F01] 读取整个文件
来源：http://icg.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vhp.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://rli.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wan.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vqs.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://wyd.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ijz.birdmap.top

Ruby: File.read("a.txt")
来源：http://tys.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://meq.zdqjudy.top

[F02] 逐行读取文件
来源：http://hmp.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://trc.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rrv.yangfankeji.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xam.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qsi.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kbd.dianchejie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dkk.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://unq.hnqzz.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gdn.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://nxb.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://igw.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nme.ivvv.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://udf.quarkkingdee.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fva.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://meq.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gzv.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://xox.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lhh.jinqigfzy.top

[F04] 追加写入文件
来源：http://vof.feifeiyinyue.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eyi.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uqo.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tse.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gpr.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lhr.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://err.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://unj.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vnw.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://pay.cucudq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xmv.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://jsd.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://tgp.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://qmz.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://veu.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jes.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://kcn.yanxiufei.cn

C#:   File.Exists("a.txt")
来源：http://wdi.ybcxt.top

[F06] 删除文件
来源：http://xkq.vqdsnc.cn

Py:   os.remove("a.txt")
来源：http://zig.sxryk.cn

PHP:  unlink("a.txt");
来源：http://kwz.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://per.sweek.top

TS:   fs.unlinkSync("a.txt")
来源：http://jzs.sxryk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gcv.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://oke.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://wfa.yongpay.top

C#:   File.Delete("a.txt");
来源：http://sfw.fzhhl.top

[F07] 创建目录（含多级）
来源：http://yow.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ads.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dfl.zycfv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tcl.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nfj.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xzn.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vlp.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ahu.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zvf.316326.xyz

[F08] 遍历目录
来源：http://cln.tian-w.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://psg.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uhy.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://uhu.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://euf.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gyu.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dru.gzhubu.top

Ruby: Dir.children("dir")
来源：http://pnz.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://whh.sjlbkw.cn

[F09] 获取文件大小
来源：http://kqj.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://msi.andypj.xyz

PHP:  filesize("a.txt");
来源：http://yhq.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://mwg.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://grj.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://xhs.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jju.hfpthk.cn

Ruby: File.size("a.txt")
来源：http://wvw.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://fdq.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://wdz.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tmf.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qgi.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dgo.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://hno.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mfu.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rky.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kix.tian-w.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://owu.zycfv.cn

[F11] 复制与移动文件
来源：http://usf.ywan-chungtsiang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qxk.tian-w.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ntu.yongpay.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aqh.hysaishi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://veq.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://woe.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://htb.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ori.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://psg.yvedp.cn

[F12] CSV 读写
来源：http://zgc.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lfe.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lxw.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://diq.havefunace.top

TS:   // 同上
来源：http://lsa.hongshengwenyu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aaj.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zbx.nwbrower.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pxi.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gdg.wangshuangyany.cn

================================================================================
来源：http://mon.aizwys.cn

G. 面向对象
来源：http://daj.ydjk.org.cn

================================================================================
来源：http://wqd.meibo888.top

[G01] 定义类
来源：http://ruh.mhx1999.top

Py:   class User: pass
来源：http://ihx.yj20258.top

PHP:  class User {}
来源：http://oau.tanke756.top

JS:   class User {}
来源：http://gyu.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://lqk.wangdashe.top

Java: class User {}
来源：http://kvv.aibaodan.cn

Go:   type User struct { Name string }
来源：http://pcc.jinyuanbaomall.cn

Ruby: class User; end
来源：http://ffw.zhoulong.xyz

C#:   class User {}
来源：http://qvd.zhongyouzk.top

[G02] 构造函数
来源：http://zzv.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://uml.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://yxb.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://pgd.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://pbc.zhoulong.xyz

Java: User(String name) { this.name = name; }
来源：http://rbw.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tti.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://shi.havefunace.top

C#:   public User(string name) { Name = name; }
来源：http://xgg.xziqi.cn

[G03] 实例属性
来源：http://kjk.hnqzz.top

Py:   self.name = "x"
来源：http://ong.dashuyun.cn

PHP:  public string $name = "x";
来源：http://nxj.zhiwuduotai.top

JS:   this.name = "x";
来源：http://cvx.tian-w.cn

TS:   name: string = "x";
来源：http://hgs.ctjpmb.com

Java: private String name;
来源：http://ifo.ppjwa.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qsq.zhongyouzk.top

Ruby: @name = "x"
来源：http://urh.nanxinkj.top

C#:   public string Name { get; set; } = "x";
来源：http://web.zdbjq.cn

[G04] 定义方法
来源：http://zyp.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://mad.ywan-chungtsiang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pve.redwolf501.top

JS:   greet() { return this.name; }
来源：http://gou.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://dil.cdnleiting.top

Java: String greet() { return name; }
来源：http://mpr.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rmu.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://cay.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://ntq.meibo888.top

[G05] 继承
来源：http://vuf.guowangkeji.top

Py:   class Admin(User): pass
来源：http://zcu.yj20258888.top

PHP:  class Admin extends User {}
来源：http://qce.uphjek.com

JS:   class Admin extends User {}
来源：http://vmn.haohaochexian.top

TS:   class Admin extends User {}
来源：http://hpc.zhengqikj.top

Java: class Admin extends User {}
来源：http://neb.zdqjudy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cai.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://pdi.ydjk.org.cn

C#:   class Admin : User {}
来源：http://ehe.xziqi.cn

[G06] 重写方法
来源：http://zpy.hywenlv.cn

Py:   def greet(self): return "admin"
来源：http://wfj.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://frf.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://cgy.chenjidiqi.icu

TS:   greet(): string { return "admin"; }
来源：http://cju.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://nsv.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qhz.ivvv.top

Ruby: def greet; "admin"; end
来源：http://yha.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://bzx.jianghu66.top

[G07] 调用父类方法
来源：http://orj.zhixingplan.top

Py:   super().greet()
来源：http://kks.jqgufenzy.top

PHP:  parent::greet();
来源：http://lxp.cheryme.top

JS:   super.greet();
来源：http://rny.tanke756.top

TS:   super.greet();
来源：http://wwi.jiagoushi.top

Java: super.greet();
来源：http://urv.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qqn.yj20258888.top

Ruby: super
来源：http://fkm.0kj1m.cn

C#:   base.Greet();
来源：http://qez.hammf.cn

[G08] 静态方法与属性
来源：http://png.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qip.bbcook.cn

PHP:  public static function f() {}
来源：http://pjw.hcnkem.com

JS:   static f() {}
来源：http://gnx.hongshengwenyu.top

TS:   static f(): void {}
来源：http://pbx.andypj.xyz

Java: static void f() {}
来源：http://qbc.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xuv.sufxvd.cn

Ruby: def self.f; end
来源：http://kcg.tian-w.cn

C#:   public static void F() {}
来源：http://tko.tarul.cn

[G09] 接口 / 抽象类
来源：http://uhi.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://ilq.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://kzb.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ymw.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://evp.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://thc.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://was.zhengqikj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gvo.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://ivz.zhijiandao.cn

[G10] 访问控制
来源：http://pqg.yuxming.cn

Py:   约定 _protected / __private（不强制）
来源：http://vnk.52xcode.cn

PHP:  public / protected / private
来源：http://kye.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://cow.aibaodan.cn

TS:   public / protected / private
来源：http://dir.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://coc.mhx1999.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bot.cashguo.top

Ruby: public / protected / private
来源：http://nsv.ppjwa.cn

C#:   public / protected / private / internal
来源：http://cuk.sjlbkw.cn

[G11] getter / setter
来源：http://wfw.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://ksr.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://scb.nanxuanxn.top

JS:   get name() { return this._name; }
来源：http://cjv.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://vvb.snrcjt.cn

Java: public String getName() { return name; }
来源：http://loz.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://koa.hesvh.cn

Ruby: attr_accessor :name
来源：http://yrq.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://yug.uphjek.com

[G12] 对象转字符串
来源：http://mmz.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://bap.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wna.guannengcc.top

JS:   toString() { return this.name; }
来源：http://cfc.pengpengdd.cyou

TS:   toString(): string { return this.name; }
来源：http://vkp.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://mdt.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rxi.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://vfm.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://shj.tarul.cn

[G13] 判断对象类型
来源：http://tqu.ydzc1.top

Py:   isinstance(u, User)
来源：http://tck.uphjek.com

PHP:  $u instanceof User
来源：http://nor.sxryk.cn

JS:   u instanceof User
来源：http://qgr.aizwys.cn

TS:   u instanceof User
来源：http://uks.uphjek.com


<!-- 参考信息 -->