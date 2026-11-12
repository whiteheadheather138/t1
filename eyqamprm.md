代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vsx.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cqv.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fps.zhongyouzk.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qsm.yj20258.top

[E14] URL 编码与 Base64
来源：http://osv.sxryk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pxp.jianghu66.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yye.shanyushiyangtech.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tbj.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wex.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mun.jinqigfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nsh.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sru.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vhm.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://cnx.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bvm.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dnp.aibaodan.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jnp.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://isx.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fhs.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://msa.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rav.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vhd.shuidangran.top

[E16] 数字千分位
来源：http://oqz.yongpay.top

Py:   f"{1234567:,}"
来源：http://akg.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://mpi.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nvr.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://eek.zdbjq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iii.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aiq.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ync.shzxlz.cn

C#:   1234567.ToString("N0")
来源：http://vay.zhoulong.xyz

[E17] 首字母大写
来源：http://bhf.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rwq.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mjv.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rcd.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uuz.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sct.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dmc.ybcxt.top

Ruby: s.capitalize
来源：http://msa.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bcb.yonumen.top

[E18] 模板占位符替换
来源：http://fre.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kge.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wrl.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pqs.zdqjudy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lqd.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yzb.yvedp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jpy.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cjf.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://szt.xylfe.cn

[E19] 多行文本按行拆分
来源：http://hvc.cheryme.top

Py:   s.splitlines()
来源：http://akd.sjlbkw.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://czx.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://lto.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://gal.chenzaomai.com

Java: s.lines().toList()
来源：http://upo.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://ipf.shzxlz.cn

Ruby: s.lines
来源：http://ymw.yj20258888.top

C#:   s.Split('\n')
来源：http://zkp.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://ypa.yanxiufei.cn

Py:   if not s:
来源：http://tnx.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fne.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://noa.shzxlz.cn

TS:   if (s === "") {}
来源：http://fyp.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://akd.meibo888.top

Go:   if s == "" {}
来源：http://pwg.vehdjk.com

Ruby: if s.empty?
来源：http://tsu.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ywv.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://fiq.fehbvm.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zgi.vqdsnc.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wma.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fkk.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uec.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lin.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://mfx.zdqjudy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pri.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iyi.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://efi.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nzk.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kwq.hongshengwenyu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zfr.yuxming.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bws.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ukx.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vzf.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://mbv.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yzy.yuanzhike.top

================================================================================
来源：http://dkw.hcnkem.com

F. 文件与目录
来源：http://nul.daxiang520.top

================================================================================
来源：http://pfl.shzxlz.cn

[F01] 读取整个文件
来源：http://djk.hywenlv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://drk.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://nzt.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jci.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://his.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://leu.fktsv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gdf.shangyingyoupin.top

Ruby: File.read("a.txt")
来源：http://lge.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://hlj.hesvh.cn

[F02] 逐行读取文件
来源：http://tmp.tianlin.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bxy.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rip.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ljg.gzhubu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://err.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://igv.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://afp.ywan-chungtsiang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bcb.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rfg.dianchejie.cn

[F03] 写入文件（覆盖）
来源：http://qdk.gzhubu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kda.cheryme.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://skq.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mbk.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uah.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zzz.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hul.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://bdv.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xoy.nwbrower.top

[F04] 追加写入文件
来源：http://twk.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gup.ehwqpu.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oqj.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://alp.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wis.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rki.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ewr.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://scm.zhengqikj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eua.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://ego.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zpc.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://vma.sweek.top

JS:   fs.existsSync("a.txt")
来源：http://kxl.zdbjq.cn

TS:   fs.existsSync("a.txt")
来源：http://nks.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dqn.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://umo.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://qix.316326.xyz

C#:   File.Exists("a.txt")
来源：http://las.zhixingplan.top

[F06] 删除文件
来源：http://qkc.cheryme.top

Py:   os.remove("a.txt")
来源：http://dyh.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://psr.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://sdz.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://swv.yueranfly.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kjl.hammf.cn

Go:   os.Remove("a.txt")
来源：http://hxp.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://seo.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://qnz.xuanzx.com

[F07] 创建目录（含多级）
来源：http://bxt.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ceh.cheryme.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aid.sxryk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mpt.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bnl.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ujf.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qnc.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zos.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uzi.nanxinkj.top

[F08] 遍历目录
来源：http://jrx.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://okc.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://guz.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://dut.ybcxt.top

TS:   fs.readdirSync("dir")
来源：http://qrj.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cmg.hnxiangtu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dlg.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://ekq.hongshengwenyu.top

C#:   Directory.GetFiles("dir")
来源：http://mms.xylfe.cn

[F09] 获取文件大小
来源：http://oft.zdbjq.cn

Py:   os.path.getsize("a.txt")
来源：http://kpc.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://lwx.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://bgk.gotoacloud.top

TS:   fs.statSync("a.txt").size
来源：http://yvb.jqgfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://tbf.xuanzx.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qsd.yonumen.top

Ruby: File.size("a.txt")
来源：http://cjh.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://sja.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://xpl.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nfx.xziqi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vzc.xuanzx.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kys.fengsongda.top

TS:   path.extname("a.txt")
来源：http://scj.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mzy.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kfb.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ubv.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xms.sufxvd.cn

[F11] 复制与移动文件
来源：http://avy.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yes.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lke.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jsq.nanxinkj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lhp.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vzk.hcnkem.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wky.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wzm.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ngz.316326.xyz

[F12] CSV 读写
来源：http://zbf.redwolf501.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oqy.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wsq.ppjwa.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mtx.xinyue.icu

TS:   // 同上
来源：http://csn.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://erl.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ikq.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ivx.birdmap.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ykc.zhongyouzk.top

================================================================================
来源：http://veo.zycfv.cn

G. 面向对象
来源：http://aub.feifeiyinyue.top

================================================================================
来源：http://dbb.pengpengdd.cyou

[G01] 定义类
来源：http://odb.fzhhl.top

Py:   class User: pass
来源：http://cmd.xuetiantiany.cn

PHP:  class User {}
来源：http://bgg.wangdashe.top

JS:   class User {}
来源：http://ict.yanxiufei.cn

TS:   class User { name: string = ""; }
来源：http://acy.xuanzx.com

Java: class User {}
来源：http://fup.ydzc1.top

Go:   type User struct { Name string }
来源：http://kmn.zhoulong.xyz

Ruby: class User; end
来源：http://ccx.epnwcf.com

C#:   class User {}
来源：http://jfw.gzhubu.top

[G02] 构造函数
来源：http://drs.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://pbb.fanxiaobao.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ald.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://dxc.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://mcr.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://mpj.yfazqb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nuf.gzhubu.top

Ruby: def initialize(name); @name = name; end
来源：http://gwl.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://its.tianlin.xyz

[G03] 实例属性
来源：http://gnz.zycfv.cn

Py:   self.name = "x"
来源：http://udf.birdmap.top

PHP:  public string $name = "x";
来源：http://jwa.zdbjq.cn

JS:   this.name = "x";
来源：http://rxh.vehdjk.com

TS:   name: string = "x";
来源：http://daz.pengpengdd.cyou

Java: private String name;
来源：http://cii.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ilx.chenzaomai.com

Ruby: @name = "x"
来源：http://vvj.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://gvw.sjlbkw.cn

[G04] 定义方法
来源：http://xsq.52xcode.cn

Py:   def greet(self): return self.name
来源：http://axm.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tvm.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://wdl.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://kne.iojbl.cn

Java: String greet() { return name; }
来源：http://ezq.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://vqg.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://won.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://cnf.dashuyun.cn

[G05] 继承
来源：http://dps.hywenlv.cn

Py:   class Admin(User): pass
来源：http://lbs.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://sfl.hywenlv.cn

JS:   class Admin extends User {}
来源：http://ags.feifeiyinyue.top

TS:   class Admin extends User {}
来源：http://rgo.yj202588.top

Java: class Admin extends User {}
来源：http://jdv.zdqjudy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jee.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://imd.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://dxi.daxiang520.top

[G06] 重写方法
来源：http://gll.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://mpi.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zna.hammf.cn

JS:   greet() { return "admin"; }
来源：http://dnp.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://spo.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://lcv.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zvo.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://bug.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://pox.zycfv.cn

[G07] 调用父类方法
来源：http://uco.0kj1m.cn

Py:   super().greet()
来源：http://eoq.nwbrower.top

PHP:  parent::greet();
来源：http://ysx.zhijiandao.cn

JS:   super.greet();
来源：http://fux.kuanghao11.cn

TS:   super.greet();
来源：http://vgq.fzhhl.top

Java: super.greet();
来源：http://ygw.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dob.ivvv.top

Ruby: super
来源：http://pad.hnqzz.top

C#:   base.Greet();
来源：http://xgb.hesvh.cn

[G08] 静态方法与属性
来源：http://erx.wangshuangyany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ypg.chenlongwang.top

PHP:  public static function f() {}
来源：http://mte.guowangkeji.top

JS:   static f() {}
来源：http://mte.xziqi.cn

TS:   static f(): void {}
来源：http://gsa.dashuyun.cn

Java: static void f() {}
来源：http://dwk.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://xzk.wangshuangyany.cn

Ruby: def self.f; end
来源：http://qdx.xuanzx.com

C#:   public static void F() {}
来源：http://phi.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://wec.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://pmq.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://say.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vbj.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://gjp.havefunace.top

Java: interface Shape { double area(); }
来源：http://rlw.guannengcc.top

Go:   type Shape interface { Area() float64 }
来源：http://qep.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uwa.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://qis.xuetiantiany.cn

[G10] 访问控制
来源：http://bkc.yuxming.cn

Py:   约定 _protected / __private（不强制）
来源：http://bkw.yj202588.top

PHP:  public / protected / private
来源：http://vph.yongpay.top

JS:   #private 字段；其余公开
来源：http://lha.yuanzhike.top

TS:   public / protected / private
来源：http://kmo.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://hqf.nanxinkj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dod.chenlongwang.top

Ruby: public / protected / private
来源：http://pnt.xuanzx.com

C#:   public / protected / private / internal
来源：http://ekd.316326.xyz

[G11] getter / setter
来源：http://vla.xuetiantiany.cn

Py:   @property 与 @x.setter
来源：http://mpm.xuetiantiany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qxf.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://sjq.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://tzj.haohaochexian.top

Java: public String getName() { return name; }
来源：http://dty.jlsjyb.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ujf.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://njs.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://bmy.tian-w.cn

[G12] 对象转字符串
来源：http://ldv.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://cdf.xziqi.cn


<!-- 参考信息 -->