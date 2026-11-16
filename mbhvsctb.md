代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iqz.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sfr.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ecc.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uyh.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bdc.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://gut.guowangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://abt.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ghg.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fnf.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gxc.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jvk.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://smm.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yof.chenlongwang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cut.yueranfly.top

[E16] 数字千分位
来源：http://vww.yonumen.top

Py:   f"{1234567:,}"
来源：http://kdi.zycfv.cn

PHP:  number_format(1234567);
来源：http://apf.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lyr.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rqq.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://olm.yongpay.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gcl.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nke.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://iky.vehdjk.com

[E17] 首字母大写
来源：http://avd.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://snb.iojbl.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zqg.0kj1m.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://omp.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gny.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gsy.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xji.yj202588.top

Ruby: s.capitalize
来源：http://jee.sufxvd.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mcv.iojbl.cn

[E18] 模板占位符替换
来源：http://vkv.xziqi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://etq.9152youxi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rcd.fengsongda.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gsq.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pcq.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dzm.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xua.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uws.sxryk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zlp.316326.xyz

[E19] 多行文本按行拆分
来源：http://uhr.sxryk.cn

Py:   s.splitlines()
来源：http://vgc.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ooi.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://gzj.dianchejie.cn

TS:   s.split(/\r?\n/)
来源：http://eqa.yvedp.cn

Java: s.lines().toList()
来源：http://lsf.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://qea.jinyuanbaomall.cn

Ruby: s.lines
来源：http://rpz.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://tfh.zhiwuduotai.top

[E20] 判断字符串是否为空
来源：http://oxg.jinghuilouyu.cn

Py:   if not s:
来源：http://mfd.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qxg.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ogb.nanxuanxn.top

TS:   if (s === "") {}
来源：http://roi.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://uun.tarul.cn

Go:   if s == "" {}
来源：http://rll.jqgufenzy.top

Ruby: if s.empty?
来源：http://rxa.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ott.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://elm.fzhhl.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yvr.zhoulong.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ofw.feifeiyinyue.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fml.yanxiufei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ons.iojbl.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vpz.jyoumei.cn

Go:   // 按 rune 判断长度后截断
来源：http://aje.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lzf.jqgfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bxa.tanke756.top

[E22] 字节长度与字符长度
来源：http://qav.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://myi.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qdt.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yrq.nanxinkj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qzb.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oaw.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vpo.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://jaa.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uis.chenlongwang.top

================================================================================
来源：http://zld.yj202588.top

F. 文件与目录
来源：http://frz.sweek.top

================================================================================
来源：http://eni.hcnkem.com

[F01] 读取整个文件
来源：http://ygu.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hqw.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://ccr.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wxj.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vil.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qey.jinqigfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ecp.mhx1999.top

Ruby: File.read("a.txt")
来源：http://eqf.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://uss.dianchejie.cn

[F02] 逐行读取文件
来源：http://srm.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hpw.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ipa.ppjwa.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ksd.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hcm.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://onm.gotoacloud.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jti.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vcz.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gse.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://azj.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aha.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jor.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vup.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ysv.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://abi.cucudq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oiv.shanyushiyangtech.top

Ruby: File.write("a.txt", "hi")
来源：http://yll.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nod.nanxuanxn.top

[F04] 追加写入文件
来源：http://bkf.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://axu.jyoumei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://smd.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oyg.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ujl.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wuv.wangdashe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oec.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ttm.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://snj.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://hxk.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bgt.tianlin.xyz

PHP:  file_exists("a.txt");
来源：http://zzs.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://wnf.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://udj.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://snj.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xfw.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://lil.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://ush.shanyushiyangkeji.top

[F06] 删除文件
来源：http://vrd.sxryk.cn

Py:   os.remove("a.txt")
来源：http://mmi.mhx1999.top

PHP:  unlink("a.txt");
来源：http://ovr.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://kem.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://veb.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pdm.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://moi.nanxinkj.top

Ruby: File.delete("a.txt")
来源：http://pcp.hnqzz.top

C#:   File.Delete("a.txt");
来源：http://ifs.fktsv.cn

[F07] 创建目录（含多级）
来源：http://twr.svipenyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bfm.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ril.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qvl.havefunace.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://obb.zhixingplan.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fnx.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://icj.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ocs.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hwn.52xcode.cn

[F08] 遍历目录
来源：http://fnq.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nvu.yvedp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sls.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://dth.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://sjq.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rap.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bwq.zhijiandao.cn

Ruby: Dir.children("dir")
来源：http://hro.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://qlw.ybcxt.top

[F09] 获取文件大小
来源：http://tkz.yuxming.cn

Py:   os.path.getsize("a.txt")
来源：http://qac.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://ycp.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://tyn.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://dww.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://khj.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lzl.gzhubu.top

Ruby: File.size("a.txt")
来源：http://xkw.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://zyj.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://tng.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://skq.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hit.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ajd.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://bai.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uxd.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wgl.xylfe.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ymo.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://crl.aibaodan.cn

[F11] 复制与移动文件
来源：http://esx.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gyt.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bgm.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yrr.0kj1m.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iyy.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jnu.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hhj.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oif.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lfj.bjfxy.top

[F12] CSV 读写
来源：http://bxt.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://asr.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://igb.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://czo.hnxiangtu.top

TS:   // 同上
来源：http://ysa.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tbo.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ubz.haohaochexian.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dyz.chenjidiqi.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://oog.xingfuxueyuan.xyz

================================================================================
来源：http://gyo.hammf.cn

G. 面向对象
来源：http://ytx.shangyingyoupin.top

================================================================================
来源：http://ffm.sjlbkw.cn

[G01] 定义类
来源：http://dfi.kuanghao11.cn

Py:   class User: pass
来源：http://pzw.yonumen.top

PHP:  class User {}
来源：http://imn.hysaishi.cn

JS:   class User {}
来源：http://glf.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://hhf.andypj.xyz

Java: class User {}
来源：http://pcf.cdnleiting.top

Go:   type User struct { Name string }
来源：http://fuj.jqgfzy.top

Ruby: class User; end
来源：http://nhg.yj202588.top

C#:   class User {}
来源：http://ehd.birdmap.top

[G02] 构造函数
来源：http://fru.cdnleiting.top

Py:   def __init__(self, name): self.name = name
来源：http://pqn.zhoulong.xyz

PHP:  public function __construct(public string $name) {}
来源：http://axm.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://nwh.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://yjh.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://gra.jinghuilouyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eng.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://den.cdnleiting.top

C#:   public User(string name) { Name = name; }
来源：http://nfl.zhongyouzk.top

[G03] 实例属性
来源：http://nld.yueranfly.top

Py:   self.name = "x"
来源：http://npf.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://otv.uphjek.com

JS:   this.name = "x";
来源：http://dth.yuanzhike.top

TS:   name: string = "x";
来源：http://ium.uphjek.com

Java: private String name;
来源：http://suw.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wpw.zhiwuduotai.top

Ruby: @name = "x"
来源：http://gep.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://zmg.ywan-chungtsiang.top

[G04] 定义方法
来源：http://vbc.mhx1999.top

Py:   def greet(self): return self.name
来源：http://oga.meibo888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rbl.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://hbm.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://jtm.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://asr.ppjwa.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://szh.daxiang520.top

Ruby: def greet; @name; end
来源：http://pku.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://nzd.c1oappe.top

[G05] 继承
来源：http://jmt.hammf.cn

Py:   class Admin(User): pass
来源：http://qsd.pycfn.com

PHP:  class Admin extends User {}
来源：http://xpy.gogol.net.cn

JS:   class Admin extends User {}
来源：http://bml.uphjek.com

TS:   class Admin extends User {}
来源：http://ndh.snrcjt.cn

Java: class Admin extends User {}
来源：http://rop.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tdz.epnwcf.com

Ruby: class Admin < User; end
来源：http://awr.hnqzz.top

C#:   class Admin : User {}
来源：http://hyu.ivvv.top

[G06] 重写方法
来源：http://lji.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://jje.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cgk.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://gjf.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://kve.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://mcl.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kjl.hnxiangtu.top

Ruby: def greet; "admin"; end
来源：http://gzy.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://hxt.pengpengdd.cyou

[G07] 调用父类方法
来源：http://xwz.cucudq.cn

Py:   super().greet()
来源：http://glo.chenlongwang.top

PHP:  parent::greet();
来源：http://zua.sjlbkw.cn

JS:   super.greet();
来源：http://jik.ctjpmb.com

TS:   super.greet();
来源：http://ddq.zhoulong.xyz

Java: super.greet();
来源：http://vdi.jinghuilouyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hks.cashguo.top

Ruby: super
来源：http://vus.shangyingyoupin.top

C#:   base.Greet();
来源：http://abh.uphjek.com

[G08] 静态方法与属性
来源：http://wub.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cnw.hywenlv.cn

PHP:  public static function f() {}
来源：http://zcu.hcnkem.com

JS:   static f() {}
来源：http://fyi.jqgfzy.top

TS:   static f(): void {}
来源：http://ilw.ppjwa.cn

Java: static void f() {}
来源：http://nax.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://kai.aizwys.cn

Ruby: def self.f; end
来源：http://dbo.zhixingplan.top

C#:   public static void F() {}
来源：http://mac.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://aqu.guannengcc.top

Py:   from abc import ABC, abstractmethod
来源：http://ezv.birdmap.top

PHP:  interface Shape { public function area(): float; }
来源：http://kuo.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rca.chenlongwang.top

TS:   interface Shape { area(): number; }
来源：http://qba.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://sgc.cashguo.top

Go:   type Shape interface { Area() float64 }
来源：http://pzs.aibaodan.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://npr.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://wgb.vehdjk.com

[G10] 访问控制
来源：http://cif.hongshengwenyu.top

Py:   约定 _protected / __private（不强制）
来源：http://amw.tanke756.top

PHP:  public / protected / private
来源：http://wge.shanyushiyangkeji.top

JS:   #private 字段；其余公开
来源：http://qcv.tanke756.top

TS:   public / protected / private
来源：http://djy.yuxming.cn

Java: public / protected / private / 默认包级
来源：http://ovl.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://ear.jinyuanbaomall.cn

Ruby: public / protected / private
来源：http://wsx.kuanghao11.cn

C#:   public / protected / private / internal
来源：http://ulu.guannengcc.top

[G11] getter / setter
来源：http://xln.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://wng.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://omr.jinqigufen.top

JS:   get name() { return this._name; }
来源：http://him.zhongyouzk.top

TS:   get name(): string { return this._name; }
来源：http://sre.jlsjyb.cn

Java: public String getName() { return name; }
来源：http://chl.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://par.ivvv.top

Ruby: attr_accessor :name
来源：http://dnj.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://ugg.fehbvm.com

[G12] 对象转字符串
来源：http://qba.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://tca.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zfi.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://fzl.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://hez.epnwcf.com

Java: @Override public String toString() { return name; }
来源：http://idv.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zjl.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://tpf.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://jck.shzxlz.cn

[G13] 判断对象类型
来源：http://pur.tarul.cn


<!-- 参考信息 -->