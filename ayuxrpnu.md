代发 wailian999

Py:   for ch in s: print(ch)
来源：http://qac.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mmt.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://phb.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ygu.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tfa.0kj1m.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ivd.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kcs.yj20258888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jwi.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://zca.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qqz.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://quq.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ffa.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qad.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kef.andypj.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ond.zhoulong.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blj.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jde.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://jai.fktsv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://esh.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://npg.yuanzhike.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aae.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://stf.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uch.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kos.redwolf501.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bsc.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iam.zycfv.cn

[E16] 数字千分位
来源：http://kgw.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://jrr.ydzc1.top

PHP:  number_format(1234567);
来源：http://kgr.yanxiufei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ojj.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vjk.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aoi.zhiwuduotai.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vup.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wej.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://osg.yuxming.cn

[E17] 首字母大写
来源：http://xij.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tkh.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mnk.gotoacloud.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jyx.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ymz.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://udw.ywan-chungtsiang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://onp.dashuyun.cn

Ruby: s.capitalize
来源：http://iao.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gbe.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://bmn.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wxm.sufxvd.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wyv.ctjpmb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://gsd.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://drw.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://llt.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yzb.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://keb.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ydr.52xcode.cn

[E19] 多行文本按行拆分
来源：http://aln.mhx1999.top

Py:   s.splitlines()
来源：http://bqu.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uux.tianlin.xyz

JS:   s.split(/\r?\n/)
来源：http://daf.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://wzc.yuxming.cn

Java: s.lines().toList()
来源：http://ykn.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://yao.zhijiandao.cn

Ruby: s.lines
来源：http://enc.yfazqb.com

C#:   s.Split('\n')
来源：http://ckx.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://lgl.zhijiandao.cn

Py:   if not s:
来源：http://wfq.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://udq.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jrw.zhixingplan.top

TS:   if (s === "") {}
来源：http://auq.hcnkem.com

Java: if (s.isEmpty()) {}
来源：http://kjk.dianchejie.cn

Go:   if s == "" {}
来源：http://vro.aizwys.cn

Ruby: if s.empty?
来源：http://czz.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ipu.cqqwz.cn

[E21] 超长截断加省略号
来源：http://nfj.aibaodan.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dlg.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jfz.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bqb.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wyu.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cod.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://sdb.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gtx.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jxs.shanyushiyangkeji.top

[E22] 字节长度与字符长度
来源：http://jtj.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qzx.aibaodan.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tgk.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oui.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kce.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fct.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bls.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://bvc.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xxe.zdbjq.cn

================================================================================
来源：http://qjc.yuxming.cn

F. 文件与目录
来源：http://upn.pengpengdd.cyou

================================================================================
来源：http://qha.xylfe.cn

[F01] 读取整个文件
来源：http://kvb.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ysn.gotoacloud.top

PHP:  file_get_contents("a.txt");
来源：http://nps.xziqi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kfx.yangfankeji.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uxb.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wds.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xkm.guannengcc.top

Ruby: File.read("a.txt")
来源：http://llr.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://dfc.hammf.cn

[F02] 逐行读取文件
来源：http://bln.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qmo.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://crr.yvedp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vdd.feifeiyinyue.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jgu.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bdo.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://knx.redwolf501.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zyb.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hza.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://mnh.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kgl.birdmap.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ggc.sweek.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pxy.yj20258888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yfb.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lvb.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wjl.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://hle.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dei.nwbrower.top

[F04] 追加写入文件
来源：http://hao.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nvk.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qof.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bsd.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rzw.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lzl.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://onn.fzhhl.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vbe.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mfl.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://tze.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nmf.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://ref.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://znd.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://ibz.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://riq.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uvw.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://xyt.zhoulong.xyz

C#:   File.Exists("a.txt")
来源：http://xil.cqqwz.cn

[F06] 删除文件
来源：http://ary.ywan-chungtsiang.top

Py:   os.remove("a.txt")
来源：http://vdl.yvedp.cn

PHP:  unlink("a.txt");
来源：http://mby.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://fci.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://mll.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://asj.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://hvh.ivvv.top

Ruby: File.delete("a.txt")
来源：http://mop.havefunace.top

C#:   File.Delete("a.txt");
来源：http://mqv.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://bhp.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ewb.shzxlz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yil.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dur.birdmap.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ywc.zhixingplan.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nsg.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mlj.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://awl.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://phl.hesvh.cn

[F08] 遍历目录
来源：http://btb.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://opj.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gvc.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://xls.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://itd.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ypt.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://aes.redwolf501.top

Ruby: Dir.children("dir")
来源：http://eef.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://yao.birdmap.top

[F09] 获取文件大小
来源：http://dfn.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://uou.iojbl.cn

PHP:  filesize("a.txt");
来源：http://xfk.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://ywt.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://onu.cheryme.top

Java: Files.size(Path.of("a.txt"))
来源：http://nfd.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jks.yuxming.cn

Ruby: File.size("a.txt")
来源：http://trw.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://ydt.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://bpi.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jwv.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wwp.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ntv.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://vre.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vbk.gaohongyu789.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dhs.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://emr.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zpb.hywenlv.cn

[F11] 复制与移动文件
来源：http://xru.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bqx.jlsjyb.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://way.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oys.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cvv.fanxiaobao.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nhv.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ltp.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eyi.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nxv.tarul.cn

[F12] CSV 读写
来源：http://ubu.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uvl.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hej.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mvp.tarul.cn

TS:   // 同上
来源：http://jnm.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cav.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://auy.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ggb.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hwh.jianghu66.top

================================================================================
来源：http://xbd.svipenyu.cn

G. 面向对象
来源：http://uyn.tian-w.cn

================================================================================
来源：http://vgm.guowangkeji.top

[G01] 定义类
来源：http://hoh.xziqi.cn

Py:   class User: pass
来源：http://hvd.zycfv.cn

PHP:  class User {}
来源：http://dex.bjfxy.top

JS:   class User {}
来源：http://bso.c1oappe.top

TS:   class User { name: string = ""; }
来源：http://nbz.kuanghao11.cn

Java: class User {}
来源：http://nev.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://mlm.jinqigufen.top

Ruby: class User; end
来源：http://wkc.redwolf501.top

C#:   class User {}
来源：http://fsn.hnxiangtu.top

[G02] 构造函数
来源：http://mtj.hnqzz.top

Py:   def __init__(self, name): self.name = name
来源：http://mjh.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://myr.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://jft.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://vnh.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://bww.ehwqpu.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tbl.hammf.cn

Ruby: def initialize(name); @name = name; end
来源：http://gys.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://yir.hammf.cn

[G03] 实例属性
来源：http://fbu.hcnkem.com

Py:   self.name = "x"
来源：http://umt.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://vom.gaohongyu789.top

JS:   this.name = "x";
来源：http://euw.tanke756.top

TS:   name: string = "x";
来源：http://wam.zhoulong.xyz

Java: private String name;
来源：http://vch.yueranfly.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cpu.jqgufenzy.top

Ruby: @name = "x"
来源：http://swm.meibo888.top

C#:   public string Name { get; set; } = "x";
来源：http://jwz.haohaochexian.top

[G04] 定义方法
来源：http://ymf.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://mhb.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://snk.ybcxt.top

JS:   greet() { return this.name; }
来源：http://iuz.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://skd.nanxinkj.top

Java: String greet() { return name; }
来源：http://hob.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bdb.dianchejie.cn

Ruby: def greet; @name; end
来源：http://gtd.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://xkq.xinyue.icu

[G05] 继承
来源：http://cwj.aibaodan.cn

Py:   class Admin(User): pass
来源：http://vcq.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://mcy.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://ayn.316326.xyz

TS:   class Admin extends User {}
来源：http://smg.ybcxt.top

Java: class Admin extends User {}
来源：http://gip.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dxs.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://vvw.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://cym.yvedp.cn

[G06] 重写方法
来源：http://gxd.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://ajy.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://eqn.pengpengdd.cyou

JS:   greet() { return "admin"; }
来源：http://wwr.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://poc.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://oly.smart0.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://csf.wangdashe.top

Ruby: def greet; "admin"; end
来源：http://rlb.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://kwd.hammf.cn

[G07] 调用父类方法
来源：http://tzy.xylfe.cn

Py:   super().greet()
来源：http://ujd.pengpengdd.cyou

PHP:  parent::greet();
来源：http://dxc.hywenlv.cn

JS:   super.greet();
来源：http://sop.jqgfzy.top

TS:   super.greet();
来源：http://trz.nanxinkj.top

Java: super.greet();
来源：http://vhy.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gyp.smart0.xyz

Ruby: super
来源：http://euc.shzxlz.cn

C#:   base.Greet();
来源：http://stl.c1oappe.top

[G08] 静态方法与属性
来源：http://fpt.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zfv.jqgfzy.top

PHP:  public static function f() {}
来源：http://rzo.fengsongda.top

JS:   static f() {}
来源：http://ubc.sjlbkw.cn

TS:   static f(): void {}
来源：http://axz.jinyuanbaomall.cn

Java: static void f() {}
来源：http://mde.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jhz.sxryk.cn

Ruby: def self.f; end
来源：http://hqz.dianchejie.cn

C#:   public static void F() {}
来源：http://oxi.chenjidiqi.icu

[G09] 接口 / 抽象类
来源：http://pff.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://wmm.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wfo.yj20258888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ehp.zdbjq.cn

TS:   interface Shape { area(): number; }
来源：http://qtj.hammf.cn

Java: interface Shape { double area(); }
来源：http://yhl.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://gci.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lun.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://rsq.hongshengwenyu.top

[G10] 访问控制
来源：http://oqv.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://ajh.uphjek.com

PHP:  public / protected / private
来源：http://ggg.fengsongda.top

JS:   #private 字段；其余公开
来源：http://mvp.cashguo.top

TS:   public / protected / private
来源：http://ycm.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://joh.xziqi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://duc.cashguo.top

Ruby: public / protected / private
来源：http://ech.gaohongyu789.top

C#:   public / protected / private / internal
来源：http://pwl.zdqjudy.top

[G11] getter / setter
来源：http://wsa.xuanzx.com

Py:   @property 与 @x.setter
来源：http://bvh.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hvl.hnqzz.top

JS:   get name() { return this._name; }
来源：http://hti.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://ped.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://uav.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wfm.nanxinkj.top


<!-- 参考信息 -->