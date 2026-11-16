代发 wailian999

PHP:  substr_count($s, "a");
来源：http://hap.iojbl.cn

JS:   s.split("a").length - 1
来源：http://tjn.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://uzl.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://glv.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://vfe.kuanghao11.cn

Ruby: s.count("a")
来源：http://tmo.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://hho.andypj.xyz

[E13] 逐字符遍历
来源：http://dbl.jinqigfzy.top

Py:   for ch in s: print(ch)
来源：http://pfb.sxryk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qdd.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kcx.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bdf.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://swc.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sps.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bhq.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://txn.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://fop.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lge.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ghl.hfpthk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qzg.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cls.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rqm.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aqa.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dmd.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xxv.xinyue.icu

[E15] HTML 转义 / 反转义
来源：http://aob.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rpu.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rax.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://epb.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lzm.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kkr.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ffc.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hgd.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aak.smart0.xyz

[E16] 数字千分位
来源：http://nyp.wangdashe.top

Py:   f"{1234567:,}"
来源：http://yss.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://pwb.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://nzc.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ojl.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sbn.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ddh.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pky.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://bcw.hcnkem.com

[E17] 首字母大写
来源：http://gxg.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hys.zhongyouzk.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://htn.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vew.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qar.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nvt.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qzw.epnwcf.com

Ruby: s.capitalize
来源：http://zjl.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://scj.sxryk.cn

[E18] 模板占位符替换
来源：http://qki.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zps.zdbjq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bqj.jinqigfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://evu.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vbn.jqgufenzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qlb.birdmap.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vja.hywenlv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ato.yangfankeji.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ign.epnwcf.com

[E19] 多行文本按行拆分
来源：http://juh.shuidangran.top

Py:   s.splitlines()
来源：http://ref.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hza.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://paa.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://tky.sjlbkw.cn

Java: s.lines().toList()
来源：http://wax.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://ywf.hongshengwenyu.top

Ruby: s.lines
来源：http://pxv.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://tqe.hnqzz.top

[E20] 判断字符串是否为空
来源：http://bcs.xylfe.cn

Py:   if not s:
来源：http://epf.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://caz.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vhq.316326.xyz

TS:   if (s === "") {}
来源：http://ahr.ybcxt.top

Java: if (s.isEmpty()) {}
来源：http://nqq.9152youxi.cn

Go:   if s == "" {}
来源：http://wqq.yuanzhike.top

Ruby: if s.empty?
来源：http://ean.gzhubu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ymr.hnqzz.top

[E21] 超长截断加省略号
来源：http://fyq.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ojs.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xgl.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://txz.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wqw.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://prr.vehdjk.com

Go:   // 按 rune 判断长度后截断
来源：http://uiv.chenzaomai.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mpm.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ovz.tarul.cn

[E22] 字节长度与字符长度
来源：http://fwd.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zrp.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kvw.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xsj.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nwf.jianghu66.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mht.zhaomingkeji.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jor.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://tny.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pxb.gotoacloud.top

================================================================================
来源：http://use.ydzc1.top

F. 文件与目录
来源：http://rtg.wangshuangyany.cn

================================================================================
来源：http://hdr.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://qwz.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fuk.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://kbn.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jue.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hpe.wangshuangyany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sdd.wangshuangyany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uml.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://yvh.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://vjx.cheryme.top

[F02] 逐行读取文件
来源：http://kax.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nmb.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aix.ppjwa.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mfg.yanxiufei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://waq.jinyuanbaomall.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lul.shanyushiyangtech.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nec.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dlz.cdnleiting.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cut.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://olq.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lfa.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tqy.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pke.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://npq.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cav.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ikv.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://hwl.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ari.xuetiantiany.cn

[F04] 追加写入文件
来源：http://mst.gogol.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ora.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ixq.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mrr.gzhubu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://evz.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hwl.cqqwz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://chu.hywenlv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hsg.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ang.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://uvw.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mpi.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://pxa.xingfuxueyuan.xyz

JS:   fs.existsSync("a.txt")
来源：http://xid.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://slh.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bjo.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://csg.zdbjq.cn

Ruby: File.exist?("a.txt")
来源：http://txr.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://cah.ydjk.org.cn

[F06] 删除文件
来源：http://enq.c1oappe.top

Py:   os.remove("a.txt")
来源：http://ery.dashuyun.cn

PHP:  unlink("a.txt");
来源：http://bss.mhx1999.top

JS:   fs.unlinkSync("a.txt")
来源：http://swh.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://cka.xinyue.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kip.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://hye.sweek.top

Ruby: File.delete("a.txt")
来源：http://bur.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://uin.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://iyp.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nta.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://atn.yvedp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://grn.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hfv.iojbl.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kdt.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://coc.bbcook.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dgg.pengpengdd.cyou

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vpn.gaohongyu789.top

[F08] 遍历目录
来源：http://ood.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pyc.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tws.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://jac.sjlbkw.cn

TS:   fs.readdirSync("dir")
来源：http://ans.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vyy.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://okz.pycfn.com

Ruby: Dir.children("dir")
来源：http://icy.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://vdl.cheryme.top

[F09] 获取文件大小
来源：http://kie.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://ari.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://jpn.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://kwp.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://may.yuanzhike.top

Java: Files.size(Path.of("a.txt"))
来源：http://amf.yuanzhike.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hgq.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://tjx.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://tep.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://soh.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nbq.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://igk.sjlbkw.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bmh.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://iww.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hhe.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eyx.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vol.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zzw.shuidangran.top

[F11] 复制与移动文件
来源：http://dmp.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qno.haohaochexian.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fnz.gotoacloud.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lwy.xylfe.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://upq.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vqn.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rbs.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jrq.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://znd.dashuyun.cn

[F12] CSV 读写
来源：http://vpt.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wrc.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cuk.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qyd.yuxming.cn

TS:   // 同上
来源：http://jdz.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://umk.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lsh.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ixj.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://lun.jinghuilouyu.cn

================================================================================
来源：http://ggp.jqgfzy.top

G. 面向对象
来源：http://dsu.ivvv.top

================================================================================
来源：http://upl.52xcode.cn

[G01] 定义类
来源：http://uch.cdnleiting.top

Py:   class User: pass
来源：http://zgo.tarul.cn

PHP:  class User {}
来源：http://gfx.zhengqikj.top

JS:   class User {}
来源：http://evf.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://zgd.ydzc1.top

Java: class User {}
来源：http://jwt.yj20258888.top

Go:   type User struct { Name string }
来源：http://dwj.zhaomingkeji.xyz

Ruby: class User; end
来源：http://xbg.daxiang520.top

C#:   class User {}
来源：http://plg.zdbjq.cn

[G02] 构造函数
来源：http://jer.fengsongda.top

Py:   def __init__(self, name): self.name = name
来源：http://lft.dashuyun.cn

PHP:  public function __construct(public string $name) {}
来源：http://agh.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://nzh.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://zvn.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://tof.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xjz.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://hox.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://bed.hesvh.cn

[G03] 实例属性
来源：http://wxx.chenzaomai.com

Py:   self.name = "x"
来源：http://zox.ehwqpu.com

PHP:  public string $name = "x";
来源：http://kyo.zhixingplan.top

JS:   this.name = "x";
来源：http://ycd.andypj.xyz

TS:   name: string = "x";
来源：http://szh.jinyuanbaomall.cn

Java: private String name;
来源：http://jbl.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cdv.yj202588.top

Ruby: @name = "x"
来源：http://lij.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://alh.yfazqb.com

[G04] 定义方法
来源：http://lzq.tarul.cn

Py:   def greet(self): return self.name
来源：http://qlh.jqgfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://imx.jianghu66.top

JS:   greet() { return this.name; }
来源：http://trs.jiagoushi.top

TS:   greet(): string { return this.name; }
来源：http://irq.fzhhl.top

Java: String greet() { return name; }
来源：http://qoi.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tbe.yj20258888.top

Ruby: def greet; @name; end
来源：http://bik.hesvh.cn

C#:   public string Greet() => Name;
来源：http://fng.zhoulong.xyz

[G05] 继承
来源：http://oec.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://qpu.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://nin.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://zgj.gotoacloud.top

TS:   class Admin extends User {}
来源：http://gxz.zhengqikj.top

Java: class Admin extends User {}
来源：http://tzs.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dxa.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://rss.snrcjt.cn

C#:   class Admin : User {}
来源：http://jga.chenjidiqi.icu

[G06] 重写方法
来源：http://oib.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://sww.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cqo.yongpay.top

JS:   greet() { return "admin"; }
来源：http://ybp.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://ayt.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://anr.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cfo.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://klv.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://hts.hammf.cn

[G07] 调用父类方法
来源：http://vjk.9152youxi.cn

Py:   super().greet()
来源：http://gxa.gotoacloud.top

PHP:  parent::greet();
来源：http://npt.jyoumei.cn

JS:   super.greet();
来源：http://lts.sxryk.cn

TS:   super.greet();
来源：http://hle.316326.xyz

Java: super.greet();
来源：http://qzy.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sim.kuanghao11.cn

Ruby: super
来源：http://gji.ivvv.top

C#:   base.Greet();
来源：http://wik.yj20258888.top

[G08] 静态方法与属性
来源：http://wri.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ert.bbcook.cn

PHP:  public static function f() {}
来源：http://duy.haohaochexian.top

JS:   static f() {}
来源：http://ynu.ppjwa.cn

TS:   static f(): void {}
来源：http://taq.chenjidiqi.icu

Java: static void f() {}
来源：http://edd.birdmap.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://orw.havefunace.top

Ruby: def self.f; end
来源：http://rfn.mhx1999.top

C#:   public static void F() {}
来源：http://luu.daria6918.cn

[G09] 接口 / 抽象类
来源：http://ojc.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://jvk.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://mpn.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://nat.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://zby.yfazqb.com

Java: interface Shape { double area(); }
来源：http://job.yfazqb.com

Go:   type Shape interface { Area() float64 }
来源：http://dze.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vbu.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://quy.guowangkeji.top

[G10] 访问控制
来源：http://ayx.yuxming.cn

Py:   约定 _protected / __private（不强制）
来源：http://dvk.ydjk.org.cn

PHP:  public / protected / private
来源：http://scn.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://avb.jqgufenzy.top

TS:   public / protected / private
来源：http://eeu.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://ocw.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yei.yuxming.cn

Ruby: public / protected / private
来源：http://hme.dianchejie.cn


<!-- 参考信息 -->