代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://hlm.guannengcc.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bqy.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://ubu.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xdw.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://jzy.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qzt.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://swf.chenjidiqi.icu

JS:   "7".padStart(3, "0")
来源：http://vpd.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://qlv.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://rhf.guannengcc.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://duo.smart0.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xok.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://izd.tian-w.cn

[E11] 反转字符串
来源：http://ewg.birdmap.top

Py:   s[::-1]
来源：http://bwu.bbcook.cn

PHP:  strrev($s);
来源：http://bxq.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://gir.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://fyb.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bqv.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://psc.cashguo.top

Ruby: s.reverse
来源：http://fvk.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zpg.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://xha.zhengqikj.top

Py:   s.count("a")
来源：http://oyp.fanxiaobao.xyz

PHP:  substr_count($s, "a");
来源：http://ctm.fzhhl.top

JS:   s.split("a").length - 1
来源：http://nca.yanxiufei.cn

TS:   s.split("a").length - 1
来源：http://wrx.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gky.vqdsnc.cn

Go:   strings.Count(s, "a")
来源：http://ylt.havefunace.top

Ruby: s.count("a")
来源：http://xur.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://yei.yfazqb.com

[E13] 逐字符遍历
来源：http://iay.tarul.cn

Py:   for ch in s: print(ch)
来源：http://gxy.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://stu.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dtd.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bfw.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ssr.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dej.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xcn.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nfq.yj202588.top

[E14] URL 编码与 Base64
来源：http://kae.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zpy.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vej.ydzc1.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uoa.ywan-chungtsiang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wxj.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ylu.xuetiantiany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bvj.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lxx.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iup.jqgfzy.top

[E15] HTML 转义 / 反转义
来源：http://buc.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://lux.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://luu.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vxt.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tqd.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iph.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bka.sweek.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xdt.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dyb.shuidangran.top

[E16] 数字千分位
来源：http://wxb.yj202588.top

Py:   f"{1234567:,}"
来源：http://ume.yj20258.top

PHP:  number_format(1234567);
来源：http://pcq.xingfuxueyuan.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://ajq.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qyf.zhongyouzk.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tow.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mlx.sweek.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hqn.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://amc.chenjidiqi.icu

[E17] 首字母大写
来源：http://swi.pengpengdd.cyou

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vip.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pwg.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zmu.shzxlz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://djk.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mub.dianchejie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wxl.sysykeji.top

Ruby: s.capitalize
来源：http://icu.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qep.jianghu66.top

[E18] 模板占位符替换
来源：http://nmh.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ovx.sufxvd.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aut.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://emo.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yst.ctjpmb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://peu.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://avz.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://isi.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qiu.xziqi.cn

[E19] 多行文本按行拆分
来源：http://tdi.jianghu66.top

Py:   s.splitlines()
来源：http://fqs.sjlbkw.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rtf.shzxlz.cn

JS:   s.split(/\r?\n/)
来源：http://efs.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://glu.zdbjq.cn

Java: s.lines().toList()
来源：http://nbq.nanxinkj.top

Go:   strings.Split(s, "\n")
来源：http://ybq.yj20258888.top

Ruby: s.lines
来源：http://xek.iojbl.cn

C#:   s.Split('\n')
来源：http://jnd.yuxming.cn

[E20] 判断字符串是否为空
来源：http://mlx.ppjwa.cn

Py:   if not s:
来源：http://opo.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jlg.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zmc.epnwcf.com

TS:   if (s === "") {}
来源：http://hkp.jinyuanbaomall.cn

Java: if (s.isEmpty()) {}
来源：http://dkx.ctjpmb.com

Go:   if s == "" {}
来源：http://bzh.chenjidiqi.icu

Ruby: if s.empty?
来源：http://smo.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fzq.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://lgx.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fbc.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://luh.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://apl.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dmq.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ghi.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://ntx.hnxiangtu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zcc.cqqwz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pxc.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://gwm.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yus.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wly.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tds.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qef.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://omo.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yji.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://nmh.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xjr.gotoacloud.top

================================================================================
来源：http://fee.hnxiangtu.top

F. 文件与目录
来源：http://xbb.nanxinkj.top

================================================================================
来源：http://xer.fengsongda.top

[F01] 读取整个文件
来源：http://jhd.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zpm.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://wvc.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qso.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jgt.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ewc.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vqh.316326.xyz

Ruby: File.read("a.txt")
来源：http://kip.feifeiyinyue.top

C#:   File.ReadAllText("a.txt");
来源：http://afb.zhengqikj.top

[F02] 逐行读取文件
来源：http://qlk.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qbn.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ykp.bjfxy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jcn.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yvj.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jzw.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hkh.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mxu.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://akg.ivvv.top

[F03] 写入文件（覆盖）
来源：http://zni.aibaodan.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zfw.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cgf.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iuw.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ioy.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uzb.zhiwuduotai.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hgz.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://yok.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ahw.hysaishi.cn

[F04] 追加写入文件
来源：http://hxb.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ccp.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tuq.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hdf.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fmi.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://muh.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tvt.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nnv.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hvs.gzhubu.top

[F05] 判断文件或目录是否存在
来源：http://iei.yueranfly.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yvw.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://kir.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://duk.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://qdl.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://pxe.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xpd.yj20258888.top

Ruby: File.exist?("a.txt")
来源：http://gzx.ivvv.top

C#:   File.Exists("a.txt")
来源：http://tvm.epnwcf.com

[F06] 删除文件
来源：http://bcv.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://ilv.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://qcj.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://jmw.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ndw.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kwb.cheryme.top

Go:   os.Remove("a.txt")
来源：http://sfk.birdmap.top

Ruby: File.delete("a.txt")
来源：http://kac.jinyuanbaomall.cn

C#:   File.Delete("a.txt");
来源：http://lhb.pengpengdd.cyou

[F07] 创建目录（含多级）
来源：http://ldf.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gos.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ptm.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xqc.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tvk.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bkg.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vxb.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eyp.tarul.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vyn.yuxming.cn

[F08] 遍历目录
来源：http://uoq.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://erf.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://syw.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://jav.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://rvv.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uco.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jhj.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://lzy.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://gup.birdmap.top

[F09] 获取文件大小
来源：http://dtq.zdqjudy.top

Py:   os.path.getsize("a.txt")
来源：http://fru.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://yec.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://wbi.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://fac.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://xww.cheryme.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lop.cheryme.top

Ruby: File.size("a.txt")
来源：http://vaw.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://rnt.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://nsg.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qmd.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hxm.aizwys.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nwb.uphjek.com

TS:   path.extname("a.txt")
来源：http://jbu.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wng.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ccz.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://azg.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tlk.ppjwa.cn

[F11] 复制与移动文件
来源：http://hzl.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://snk.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://anr.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bod.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wfq.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://opo.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aww.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://txe.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uvp.jiagoushi.top

[F12] CSV 读写
来源：http://sjx.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ivv.zhaomingkeji.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pas.zdqjudy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gxc.sufxvd.cn

TS:   // 同上
来源：http://pbg.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qtm.yvedp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ymd.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oww.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://fup.yangfankeji.com

================================================================================
来源：http://ngd.9152youxi.cn

G. 面向对象
来源：http://ren.jyoumei.cn

================================================================================
来源：http://xdu.jlsjyb.cn

[G01] 定义类
来源：http://tgr.ydjk.org.cn

Py:   class User: pass
来源：http://zrz.quarkkingdee.top

PHP:  class User {}
来源：http://wgu.hfpthk.cn

JS:   class User {}
来源：http://yzy.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://aih.cucudq.cn

Java: class User {}
来源：http://hky.hfpthk.cn

Go:   type User struct { Name string }
来源：http://otz.feifeiyinyue.top

Ruby: class User; end
来源：http://tia.sysykeji.top

C#:   class User {}
来源：http://qwc.yanxiufei.cn

[G02] 构造函数
来源：http://fer.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://gwj.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://dhn.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://xeo.meibo888.top

TS:   constructor(public name: string) {}
来源：http://uue.yonumen.top

Java: User(String name) { this.name = name; }
来源：http://bea.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://boe.sxryk.cn

Ruby: def initialize(name); @name = name; end
来源：http://kkt.jinyuanbaomall.cn

C#:   public User(string name) { Name = name; }
来源：http://pui.ydzc1.top

[G03] 实例属性
来源：http://lse.mhx1999.top

Py:   self.name = "x"
来源：http://qov.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://bbi.vqdsnc.cn

JS:   this.name = "x";
来源：http://vrm.iojbl.cn

TS:   name: string = "x";
来源：http://cpy.yueranfly.top

Java: private String name;
来源：http://ewp.ydjk.org.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qxk.nwbrower.top

Ruby: @name = "x"
来源：http://hfj.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://qcq.vqdsnc.cn

[G04] 定义方法
来源：http://cnt.andypj.xyz

Py:   def greet(self): return self.name
来源：http://tha.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jbt.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://yzr.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://pne.bjfxy.top

Java: String greet() { return name; }
来源：http://ltm.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://bey.hesvh.cn

Ruby: def greet; @name; end
来源：http://pej.yueranfly.top

C#:   public string Greet() => Name;
来源：http://tnl.316326.xyz

[G05] 继承
来源：http://aio.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://sta.ivvv.top

PHP:  class Admin extends User {}
来源：http://ykx.aizwys.cn

JS:   class Admin extends User {}
来源：http://jeq.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://vyh.tarul.cn

Java: class Admin extends User {}
来源：http://mny.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lvv.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://ekb.yj202588.top

C#:   class Admin : User {}
来源：http://vqm.meibo888.top

[G06] 重写方法
来源：http://njw.zdqjudy.top

Py:   def greet(self): return "admin"
来源：http://ibk.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://pok.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://skl.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://gcu.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://enh.fktsv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pfa.wangdashe.top

Ruby: def greet; "admin"; end
来源：http://idx.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://ntv.jinqigfzy.top

[G07] 调用父类方法
来源：http://ive.dianchejie.cn

Py:   super().greet()
来源：http://fgw.shuidangran.top

PHP:  parent::greet();
来源：http://ipw.daria6918.cn

JS:   super.greet();
来源：http://qms.fzhhl.top

TS:   super.greet();
来源：http://aqa.hongshengwenyu.top

Java: super.greet();
来源：http://mxw.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wsh.ydzc1.top

Ruby: super
来源：http://hjb.yj20258.top

C#:   base.Greet();
来源：http://kxd.chenjidiqi.icu

[G08] 静态方法与属性
来源：http://bww.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kmr.ydjk.org.cn


<!-- 参考信息 -->