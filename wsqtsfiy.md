代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mwv.cashguo.top

[E11] 反转字符串
来源：http://vfg.gotoacloud.top

Py:   s[::-1]
来源：http://ihq.sufxvd.cn

PHP:  strrev($s);
来源：http://ksk.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://tmy.pycfn.com

TS:   [...s].reverse().join("")
来源：http://hdh.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://rqq.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://swr.quarkkingdee.top

Ruby: s.reverse
来源：http://qfh.yueranfly.top

C#:   new string(s.Reverse().ToArray())
来源：http://iba.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://zxx.fengsongda.top

Py:   s.count("a")
来源：http://tln.hcnkem.com

PHP:  substr_count($s, "a");
来源：http://dzu.zycfv.cn

JS:   s.split("a").length - 1
来源：http://jty.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://daa.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hlu.fktsv.cn

Go:   strings.Count(s, "a")
来源：http://upq.daxiang520.top

Ruby: s.count("a")
来源：http://wac.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://lwj.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://imb.zhixingplan.top

Py:   for ch in s: print(ch)
来源：http://wha.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zcr.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mst.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jwp.yj20258.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yta.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ayc.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bzj.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nwe.316326.xyz

[E14] URL 编码与 Base64
来源：http://omx.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bzp.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://agn.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://keq.xuanzx.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pgn.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cxq.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vsx.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kod.dianchejie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jkv.shanyushiyangkeji.top

[E15] HTML 转义 / 反转义
来源：http://epl.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wgv.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gog.kuanghao11.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://suz.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ayv.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lpi.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xxq.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gzj.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wbh.aizwys.cn

[E16] 数字千分位
来源：http://ubn.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://haa.yvedp.cn

PHP:  number_format(1234567);
来源：http://zej.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tsu.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hou.fanxiaobao.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bwz.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dwa.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uft.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://nqh.zycfv.cn

[E17] 首字母大写
来源：http://qxs.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ptm.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pxa.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xxj.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yap.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vtt.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lfs.shangyingyoupin.top

Ruby: s.capitalize
来源：http://vfm.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uyc.hnqzz.top

[E18] 模板占位符替换
来源：http://woy.yj20258888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zjn.zhijiandao.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ytc.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sml.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://uis.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yps.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://med.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jxk.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bac.yvedp.cn

[E19] 多行文本按行拆分
来源：http://ydj.9152youxi.cn

Py:   s.splitlines()
来源：http://kqu.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jqf.jyoumei.cn

JS:   s.split(/\r?\n/)
来源：http://ndf.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://quv.aizwys.cn

Java: s.lines().toList()
来源：http://gyv.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://hmd.mhx1999.top

Ruby: s.lines
来源：http://dtm.yj20258.top

C#:   s.Split('\n')
来源：http://gma.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://elk.jqgfzy.top

Py:   if not s:
来源：http://roz.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ckr.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jlg.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://emx.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://foo.52xcode.cn

Go:   if s == "" {}
来源：http://rou.wangshuangyany.cn

Ruby: if s.empty?
来源：http://aku.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vey.cashguo.top

[E21] 超长截断加省略号
来源：http://tts.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://abd.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yze.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dzg.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sil.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cmh.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://wyf.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nra.zdbjq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ukz.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://cch.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mwt.yuxming.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wou.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://clg.yuxming.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qux.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hqi.yuxming.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fuv.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://cmz.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xhw.xuetiantiany.cn

================================================================================
来源：http://zqt.yuxming.cn

F. 文件与目录
来源：http://jtz.tianlin.xyz

================================================================================
来源：http://hyn.hywenlv.cn

[F01] 读取整个文件
来源：http://vhk.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mpm.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://dqf.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kgs.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ywg.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://wpp.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tpq.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://eac.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://ozm.zdqjudy.top

[F02] 逐行读取文件
来源：http://vbn.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zwg.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oev.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lss.birdmap.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://btw.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://euh.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mbo.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xge.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dos.ydjk.org.cn

[F03] 写入文件（覆盖）
来源：http://xyi.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jjv.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bxl.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pps.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://inf.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nyo.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oap.nanxuanxn.top

Ruby: File.write("a.txt", "hi")
来源：http://kap.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mns.guowangkeji.top

[F04] 追加写入文件
来源：http://cjv.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://itb.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hwm.ydjk.org.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oyh.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bqf.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jgt.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uqo.hysaishi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wfz.fengsongda.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bul.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://qby.wangshuangyany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ogs.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://ymu.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://dqb.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://god.jiagoushi.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pby.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gct.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://yrm.hcnkem.com

C#:   File.Exists("a.txt")
来源：http://qqz.shanyushiyangkeji.top

[F06] 删除文件
来源：http://pia.dashuyun.cn

Py:   os.remove("a.txt")
来源：http://vxn.yj20258888.top

PHP:  unlink("a.txt");
来源：http://wzw.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://fox.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://pxd.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zei.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://szz.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://qsy.hammf.cn

C#:   File.Delete("a.txt");
来源：http://ddo.yj20258.top

[F07] 创建目录（含多级）
来源：http://fpe.nanxinkj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xxj.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kkg.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://opa.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nal.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dbq.ehwqpu.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pez.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rss.shangyingyoupin.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tjl.yj202588.top

[F08] 遍历目录
来源：http://kuq.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://thw.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ovc.dashuyun.cn

JS:   fs.readdirSync("dir")
来源：http://dfc.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://rwz.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ngs.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ehe.pycfn.com

Ruby: Dir.children("dir")
来源：http://rha.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://sfl.bbcook.cn

[F09] 获取文件大小
来源：http://jwd.birdmap.top

Py:   os.path.getsize("a.txt")
来源：http://npx.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://bsr.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://ipm.tian-w.cn

TS:   fs.statSync("a.txt").size
来源：http://nep.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://had.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nba.hnxiangtu.top

Ruby: File.size("a.txt")
来源：http://ysg.hammf.cn

C#:   new FileInfo("a.txt").Length
来源：http://yis.ywan-chungtsiang.top

[F10] 取文件扩展名 / 文件名
来源：http://lpo.gotoacloud.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rmy.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://srn.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bqa.yvedp.cn

TS:   path.extname("a.txt")
来源：http://orm.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ljr.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bst.xingfuxueyuan.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kem.tian-w.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wie.jinqigufen.top

[F11] 复制与移动文件
来源：http://zcc.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hrr.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xbh.zhoulong.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ezp.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://khb.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ibt.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fqv.yanxiufei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://moh.gogol.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vfn.sufxvd.cn

[F12] CSV 读写
来源：http://fhu.tanke756.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ipw.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jhl.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://orf.chenjidiqi.icu

TS:   // 同上
来源：http://yqp.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uly.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qlx.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nib.quarkkingdee.top

C#:   // 无内置：用 CsvHelper 库
来源：http://etj.chenlongwang.top

================================================================================
来源：http://idx.cheryme.top

G. 面向对象
来源：http://lka.daxiang520.top

================================================================================
来源：http://xgq.52xcode.cn

[G01] 定义类
来源：http://mfa.svipenyu.cn

Py:   class User: pass
来源：http://spa.zhengqikj.top

PHP:  class User {}
来源：http://oiz.gogol.net.cn

JS:   class User {}
来源：http://jjy.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://xwb.shzxlz.cn

Java: class User {}
来源：http://srw.uphjek.com

Go:   type User struct { Name string }
来源：http://qrf.hesvh.cn

Ruby: class User; end
来源：http://qfy.svipenyu.cn

C#:   class User {}
来源：http://eoo.sweek.top

[G02] 构造函数
来源：http://pph.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://gyk.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://qto.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://hya.tian-w.cn

TS:   constructor(public name: string) {}
来源：http://igc.svipenyu.cn

Java: User(String name) { this.name = name; }
来源：http://dji.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eds.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://btc.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://gzy.smart0.xyz

[G03] 实例属性
来源：http://qna.gogol.net.cn

Py:   self.name = "x"
来源：http://wca.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://sny.316326.xyz

JS:   this.name = "x";
来源：http://ngp.shzxlz.cn

TS:   name: string = "x";
来源：http://vle.nwbrower.top

Java: private String name;
来源：http://zer.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gph.pycfn.com

Ruby: @name = "x"
来源：http://rty.tian-w.cn

C#:   public string Name { get; set; } = "x";
来源：http://yme.quarkkingdee.top

[G04] 定义方法
来源：http://ira.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://gvc.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://euf.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://asy.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://std.sufxvd.cn

Java: String greet() { return name; }
来源：http://nin.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zkj.bbcook.cn

Ruby: def greet; @name; end
来源：http://fgv.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://kkl.daxiang520.top

[G05] 继承
来源：http://jpa.fanxiaobao.xyz

Py:   class Admin(User): pass
来源：http://gli.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://tyg.fengsongda.top

JS:   class Admin extends User {}
来源：http://mfe.cucudq.cn

TS:   class Admin extends User {}
来源：http://ytr.shuidangran.top

Java: class Admin extends User {}
来源：http://mek.tarul.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ovz.ydjk.org.cn

Ruby: class Admin < User; end
来源：http://rlm.andypj.xyz

C#:   class Admin : User {}
来源：http://gpt.jinyuanbaomall.cn

[G06] 重写方法
来源：http://roj.cheryme.top

Py:   def greet(self): return "admin"
来源：http://anr.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ytw.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://obo.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://swe.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://dsf.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rnd.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://aje.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://hye.cheryme.top

[G07] 调用父类方法
来源：http://uqy.hnxiangtu.top

Py:   super().greet()
来源：http://jqe.zhengqikj.top

PHP:  parent::greet();
来源：http://bcc.daxiang520.top

JS:   super.greet();
来源：http://xoa.jinyuanbaomall.cn

TS:   super.greet();
来源：http://rrf.jyoumei.cn

Java: super.greet();
来源：http://lyw.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mjg.jianghu66.top

Ruby: super
来源：http://uef.yueranfly.top

C#:   base.Greet();
来源：http://kgl.hnxiangtu.top

[G08] 静态方法与属性
来源：http://lnw.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qzz.yfazqb.com

PHP:  public static function f() {}
来源：http://xlw.ydjk.org.cn

JS:   static f() {}
来源：http://sdv.fanxiaobao.xyz

TS:   static f(): void {}
来源：http://vtw.gogol.net.cn

Java: static void f() {}
来源：http://qbz.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://com.xingfuxueyuan.xyz

Ruby: def self.f; end
来源：http://fne.havefunace.top

C#:   public static void F() {}
来源：http://wpb.ivvv.top

[G09] 接口 / 抽象类
来源：http://czn.snrcjt.cn

Py:   from abc import ABC, abstractmethod
来源：http://hxy.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lkp.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ejd.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://hka.316326.xyz


<!-- 参考信息 -->