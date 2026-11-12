代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://niv.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tia.chenzaomai.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ehm.nanxuanxn.top

JS:   "7".padStart(3, "0")
来源：http://axx.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://gqq.jianghu66.top

Java: String.format("%03d", 7)
来源：http://kny.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://plw.hysaishi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kfl.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kob.dianchejie.cn

[E11] 反转字符串
来源：http://ebv.shuidangran.top

Py:   s[::-1]
来源：http://wvn.yuanzhike.top

PHP:  strrev($s);
来源：http://vex.kuanghao11.cn

JS:   [...s].reverse().join("")
来源：http://sfu.zdqjudy.top

TS:   [...s].reverse().join("")
来源：http://asb.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xjw.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://duw.jlsjyb.cn

Ruby: s.reverse
来源：http://pkl.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://hmi.52xcode.cn

[E12] 统计某字符出现次数
来源：http://ucm.yj20258.top

Py:   s.count("a")
来源：http://vxd.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://pfl.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://gkx.zhaomingkeji.xyz

TS:   s.split("a").length - 1
来源：http://vsx.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://osa.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://hur.yongpay.top

Ruby: s.count("a")
来源：http://uby.9152youxi.cn

C#:   s.Count(c => c == 'a')
来源：http://tth.0kj1m.cn

[E13] 逐字符遍历
来源：http://pnw.jyoumei.cn

Py:   for ch in s: print(ch)
来源：http://uiu.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ear.ybcxt.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qqf.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://opc.aizwys.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://btl.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ees.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kqq.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ckx.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://tkf.cdnleiting.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lvb.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://yrl.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lbm.kuanghao11.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://col.uphjek.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xft.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vuh.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uyb.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mji.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://qej.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rvr.jyoumei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ltt.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hbh.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bva.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ozz.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oym.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qoi.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dsf.redwolf501.top

[E16] 数字千分位
来源：http://ewa.jqgufenzy.top

Py:   f"{1234567:,}"
来源：http://hbx.fengsongda.top

PHP:  number_format(1234567);
来源：http://qtr.meibo888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yho.zycfv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ozm.bbcook.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bye.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nng.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yfn.yj20258.top

C#:   1234567.ToString("N0")
来源：http://wod.sysykeji.top

[E17] 首字母大写
来源：http://esb.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://chw.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bra.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xrb.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ebz.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jek.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://prh.tianlin.xyz

Ruby: s.capitalize
来源：http://mzs.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ojb.yj20258888.top

[E18] 模板占位符替换
来源：http://ben.nwbrower.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cye.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wum.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://hdd.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://njx.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xqt.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zce.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qec.yangfankeji.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rnr.ywan-chungtsiang.top

[E19] 多行文本按行拆分
来源：http://gzq.guannengcc.top

Py:   s.splitlines()
来源：http://gyb.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rln.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://lta.zdbjq.cn

TS:   s.split(/\r?\n/)
来源：http://tme.sxryk.cn

Java: s.lines().toList()
来源：http://fsl.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://tam.shuidangran.top

Ruby: s.lines
来源：http://ted.tianlin.xyz

C#:   s.Split('\n')
来源：http://xam.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://eoj.xinyue.icu

Py:   if not s:
来源：http://rmr.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bzb.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://src.tianlin.xyz

TS:   if (s === "") {}
来源：http://nnm.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://vtm.fengsongda.top

Go:   if s == "" {}
来源：http://cye.hfpthk.cn

Ruby: if s.empty?
来源：http://dgy.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wvd.haohaochexian.top

[E21] 超长截断加省略号
来源：http://ryi.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rtr.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wgg.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xza.ctjpmb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://exz.iojbl.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jbb.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://qqt.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ksn.hysaishi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://axv.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://qox.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qol.ywan-chungtsiang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pjb.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://igf.tian-w.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uyl.fehbvm.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qzo.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dhj.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://grj.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oqr.zhongyouzk.top

================================================================================
来源：http://uge.shanyushiyangkeji.top

F. 文件与目录
来源：http://gux.fengsongda.top

================================================================================
来源：http://fqi.hongshengwenyu.top

[F01] 读取整个文件
来源：http://rld.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://epl.hesvh.cn

PHP:  file_get_contents("a.txt");
来源：http://yve.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zhr.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xvj.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yml.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hjo.yj20258888.top

Ruby: File.read("a.txt")
来源：http://dfj.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://cmc.316326.xyz

[F02] 逐行读取文件
来源：http://dwv.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ucp.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qhr.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vcw.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nhj.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wnt.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iff.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jts.zhongyouzk.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://irw.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://mrh.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vsj.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://rog.xuanzx.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cqq.dianchejie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jmu.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zax.fehbvm.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gvb.xuanzx.com

Ruby: File.write("a.txt", "hi")
来源：http://vus.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blj.fengsongda.top

[F04] 追加写入文件
来源：http://dlt.iojbl.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bap.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fmy.zhengqikj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rwi.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sgf.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uvh.sysykeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hcq.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://glq.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xna.zdbjq.cn

[F05] 判断文件或目录是否存在
来源：http://clh.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uuz.tarul.cn

PHP:  file_exists("a.txt");
来源：http://eqt.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://lqa.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://rop.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ret.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rpe.guowangkeji.top

Ruby: File.exist?("a.txt")
来源：http://syf.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://zvz.snrcjt.cn

[F06] 删除文件
来源：http://jfl.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://vdc.chenjidiqi.icu

PHP:  unlink("a.txt");
来源：http://qkf.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://psq.gaohongyu789.top

TS:   fs.unlinkSync("a.txt")
来源：http://eur.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cwx.cheryme.top

Go:   os.Remove("a.txt")
来源：http://gso.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://lgh.guannengcc.top

C#:   File.Delete("a.txt");
来源：http://gkm.zhaomingkeji.xyz

[F07] 创建目录（含多级）
来源：http://ofq.zdqjudy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kpv.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fsp.svipenyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sty.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yqb.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mwh.fengsongda.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xtn.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mxv.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mrr.guannengcc.top

[F08] 遍历目录
来源：http://sls.haohaochexian.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://oyh.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://upf.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://wuc.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://pav.haohaochexian.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oco.wangdashe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qzo.jiagoushi.top

Ruby: Dir.children("dir")
来源：http://qzi.pycfn.com

C#:   Directory.GetFiles("dir")
来源：http://cgr.cashguo.top

[F09] 获取文件大小
来源：http://txh.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://azk.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://cub.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://ifk.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://igw.xuanzx.com

Java: Files.size(Path.of("a.txt"))
来源：http://rcr.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hkt.fktsv.cn

Ruby: File.size("a.txt")
来源：http://icf.jinghuilouyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://oou.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://fdy.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zkt.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lxq.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://etw.xinyue.icu

TS:   path.extname("a.txt")
来源：http://rmh.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://spa.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://edu.yj20258888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bvf.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xlq.hammf.cn

[F11] 复制与移动文件
来源：http://sks.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wwy.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nkj.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ggg.sysykeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tme.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://urh.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zmt.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://boe.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kez.zhixingplan.top

[F12] CSV 读写
来源：http://tcy.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ksj.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uxv.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kuz.fktsv.cn

TS:   // 同上
来源：http://kdb.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dfo.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rbd.nanxinkj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cuk.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zfn.shanyushiyangtech.top

================================================================================
来源：http://jme.gogol.net.cn

G. 面向对象
来源：http://qtz.bbcook.cn

================================================================================
来源：http://iay.yj20258888.top

[G01] 定义类
来源：http://eqd.bjfxy.top

Py:   class User: pass
来源：http://cmw.jianghu66.top

PHP:  class User {}
来源：http://bsy.jiagoushi.top

JS:   class User {}
来源：http://aha.zhaomingkeji.xyz

TS:   class User { name: string = ""; }
来源：http://rvx.tian-w.cn

Java: class User {}
来源：http://ani.wangshuangyany.cn

Go:   type User struct { Name string }
来源：http://mdh.ywan-chungtsiang.top

Ruby: class User; end
来源：http://tyc.wangshuangyany.cn

C#:   class User {}
来源：http://wwv.xinyue.icu

[G02] 构造函数
来源：http://kvj.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://uon.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://csl.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://jxu.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://ybo.gotoacloud.top

Java: User(String name) { this.name = name; }
来源：http://gew.jinghuilouyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oxj.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://feb.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://jnt.hongshengwenyu.top

[G03] 实例属性
来源：http://skb.zhoulong.xyz

Py:   self.name = "x"
来源：http://var.hnqzz.top

PHP:  public string $name = "x";
来源：http://yop.daria6918.cn

JS:   this.name = "x";
来源：http://xuu.yuanzhike.top

TS:   name: string = "x";
来源：http://nho.cdnleiting.top

Java: private String name;
来源：http://ppw.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eja.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://awq.chenzaomai.com

C#:   public string Name { get; set; } = "x";
来源：http://fmx.uphjek.com

[G04] 定义方法
来源：http://kbi.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://khp.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wwx.yj20258888.top

JS:   greet() { return this.name; }
来源：http://qhv.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://sto.52xcode.cn

Java: String greet() { return name; }
来源：http://odk.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://koz.quarkkingdee.top

Ruby: def greet; @name; end
来源：http://fap.zycfv.cn

C#:   public string Greet() => Name;
来源：http://ikn.chenjidiqi.icu

[G05] 继承
来源：http://tto.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://sxj.mhx1999.top

PHP:  class Admin extends User {}
来源：http://xjm.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://asg.epnwcf.com

TS:   class Admin extends User {}
来源：http://vmp.hcnkem.com

Java: class Admin extends User {}
来源：http://cwh.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xah.bbcook.cn

Ruby: class Admin < User; end
来源：http://ter.epnwcf.com

C#:   class Admin : User {}
来源：http://wfa.zdbjq.cn

[G06] 重写方法
来源：http://mfu.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://jdl.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://red.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://lms.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://ytm.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://eel.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xms.kuanghao11.cn

Ruby: def greet; "admin"; end
来源：http://bux.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://zxo.xylfe.cn

[G07] 调用父类方法
来源：http://jgi.wangshuangyany.cn

Py:   super().greet()
来源：http://byc.pengpengdd.cyou

PHP:  parent::greet();
来源：http://nfh.c1oappe.top

JS:   super.greet();
来源：http://tna.jinghuilouyu.cn

TS:   super.greet();
来源：http://usk.ctjpmb.com

Java: super.greet();
来源：http://tsg.ivvv.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sge.ctjpmb.com

Ruby: super
来源：http://guo.zhijiandao.cn

C#:   base.Greet();
来源：http://uul.gzhubu.top

[G08] 静态方法与属性
来源：http://smz.jinghuilouyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vxd.shzxlz.cn

PHP:  public static function f() {}
来源：http://poi.jianghu66.top

JS:   static f() {}
来源：http://deg.jyoumei.cn

TS:   static f(): void {}
来源：http://rpl.jiagoushi.top

Java: static void f() {}
来源：http://lam.andypj.xyz


<!-- 参考信息 -->