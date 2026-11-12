代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vbs.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://thy.yj202588.top

JS:   s.replace(/\s+/g, "")
来源：http://okk.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://sav.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://oaj.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://guj.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://epa.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wsz.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://vzc.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ens.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rqo.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://clr.fktsv.cn

TS:   "7".padStart(3, "0")
来源：http://ohg.yvedp.cn

Java: String.format("%03d", 7)
来源：http://ccv.hnqzz.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mpa.zhaomingkeji.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://voh.hongshengwenyu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tzh.ppjwa.cn

[E11] 反转字符串
来源：http://ypu.sysykeji.top

Py:   s[::-1]
来源：http://hwe.xuetiantiany.cn

PHP:  strrev($s);
来源：http://iyv.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://tfq.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://nlc.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qcy.vqdsnc.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jpw.hongshengwenyu.top

Ruby: s.reverse
来源：http://qwo.fzhhl.top

C#:   new string(s.Reverse().ToArray())
来源：http://rfb.hcnkem.com

[E12] 统计某字符出现次数
来源：http://qlm.nwbrower.top

Py:   s.count("a")
来源：http://wok.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://gjq.cucudq.cn

JS:   s.split("a").length - 1
来源：http://kcc.xuanzx.com

TS:   s.split("a").length - 1
来源：http://rnr.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ywu.gogol.net.cn

Go:   strings.Count(s, "a")
来源：http://oib.yueranfly.top

Ruby: s.count("a")
来源：http://cez.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://bqv.fehbvm.com

[E13] 逐字符遍历
来源：http://jny.zhixingplan.top

Py:   for ch in s: print(ch)
来源：http://dyn.daxiang520.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bez.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sqx.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nky.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xgz.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jiz.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://aas.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yfa.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://omo.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dwh.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hif.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fqa.cucudq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://css.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rjv.dashuyun.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tsw.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jcr.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jfw.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://xnr.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://onv.bjfxy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vgx.xylfe.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jjk.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hrz.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hzz.tianlin.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gmm.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://llx.zhongyouzk.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hpm.jinqigfzy.top

[E16] 数字千分位
来源：http://hbt.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://eef.vehdjk.com

PHP:  number_format(1234567);
来源：http://tii.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vgo.cqqwz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wyb.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://egb.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bfs.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qfv.yj202588.top

C#:   1234567.ToString("N0")
来源：http://ziq.tianlin.xyz

[E17] 首字母大写
来源：http://bbh.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pvi.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mgt.0kj1m.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tbz.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sds.jinyuanbaomall.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lbr.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qfa.fehbvm.com

Ruby: s.capitalize
来源：http://agj.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jlj.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://lvp.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://upx.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://znk.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fle.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://dbg.shangyingyoupin.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bfs.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mtn.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qsj.jinqigfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://owb.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://ije.epnwcf.com

Py:   s.splitlines()
来源：http://mho.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jxi.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://ajb.fengsongda.top

TS:   s.split(/\r?\n/)
来源：http://wvg.ydzc1.top

Java: s.lines().toList()
来源：http://yus.dashuyun.cn

Go:   strings.Split(s, "\n")
来源：http://kll.bjfxy.top

Ruby: s.lines
来源：http://rpx.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://ove.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://pvx.dianchejie.cn

Py:   if not s:
来源：http://gzc.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lhz.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ujs.sjlbkw.cn

TS:   if (s === "") {}
来源：http://qaz.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://ttw.sxryk.cn

Go:   if s == "" {}
来源：http://dkx.jinqigfzy.top

Ruby: if s.empty?
来源：http://byt.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tzp.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://vyy.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eew.cheryme.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rzj.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mhh.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ueb.cdnleiting.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ljn.zhiwuduotai.top

Go:   // 按 rune 判断长度后截断
来源：http://zqk.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hzt.jinyuanbaomall.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hsw.jinyuanbaomall.cn

[E22] 字节长度与字符长度
来源：http://att.sxryk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yyo.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aud.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qsy.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lmi.chenlongwang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eqy.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gww.tarul.cn

Ruby: s.bytesize;  s.length
来源：http://isi.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bxg.zycfv.cn

================================================================================
来源：http://odr.ctjpmb.com

F. 文件与目录
来源：http://jox.ppjwa.cn

================================================================================
来源：http://wis.yuanzhike.top

[F01] 读取整个文件
来源：http://iqo.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mzj.epnwcf.com

PHP:  file_get_contents("a.txt");
来源：http://xay.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ssj.shanyushiyangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sch.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ucp.jinyuanbaomall.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vba.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://pwd.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://zyu.jiagoushi.top

[F02] 逐行读取文件
来源：http://njz.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xsx.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://omt.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mls.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xqg.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qau.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jnn.daria6918.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qwr.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://frr.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://gta.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bsk.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://esb.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nvq.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://erf.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://svu.svipenyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vho.jianghu66.top

Ruby: File.write("a.txt", "hi")
来源：http://siy.quarkkingdee.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://crf.uphjek.com

[F04] 追加写入文件
来源：http://jwb.yonumen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tpf.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://awu.shanyushiyangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bjz.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qzv.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ubv.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gex.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rlt.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hss.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://tnz.yangfankeji.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://twm.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://xqx.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://ime.chenjidiqi.icu

TS:   fs.existsSync("a.txt")
来源：http://wyu.0kj1m.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://utx.hongshengwenyu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vih.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://hzw.gaohongyu789.top

C#:   File.Exists("a.txt")
来源：http://cpm.zhengqikj.top

[F06] 删除文件
来源：http://ubw.ybcxt.top

Py:   os.remove("a.txt")
来源：http://biq.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://adx.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://cwu.fanxiaobao.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://jok.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jiq.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://yuw.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://gka.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://qis.xziqi.cn

[F07] 创建目录（含多级）
来源：http://cmy.aizwys.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lvw.zdqjudy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kgb.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gyq.fktsv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dra.smart0.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jai.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yrj.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://can.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://opp.vqdsnc.cn

[F08] 遍历目录
来源：http://qxl.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wnh.jinqigfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nwj.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://vyb.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://czj.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bjr.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mty.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://qcz.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://fmk.zhijiandao.cn

[F09] 获取文件大小
来源：http://usw.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://sad.hnqzz.top

PHP:  filesize("a.txt");
来源：http://uhb.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://cfy.ehwqpu.com

TS:   fs.statSync("a.txt").size
来源：http://kmy.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cqc.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bvw.hcnkem.com

Ruby: File.size("a.txt")
来源：http://rct.zhijiandao.cn

C#:   new FileInfo("a.txt").Length
来源：http://hea.vqdsnc.cn

[F10] 取文件扩展名 / 文件名
来源：http://ixx.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qrc.zhoulong.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jjs.redwolf501.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vna.mhx1999.top

TS:   path.extname("a.txt")
来源：http://ggv.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jnu.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://roo.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xyc.yonumen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gbr.jianghu66.top

[F11] 复制与移动文件
来源：http://vda.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mse.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uic.zhiwuduotai.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tmo.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://itt.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fbt.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nkp.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ind.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lum.guannengcc.top

[F12] CSV 读写
来源：http://pwn.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zil.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://evw.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hph.tianlin.xyz

TS:   // 同上
来源：http://hou.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qeb.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ayy.zhoulong.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dij.yonumen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ukx.yanxiufei.cn

================================================================================
来源：http://ktl.cashguo.top

G. 面向对象
来源：http://vef.birdmap.top

================================================================================
来源：http://nkc.bjfxy.top

[G01] 定义类
来源：http://cxa.hnxiangtu.top

Py:   class User: pass
来源：http://osu.svipenyu.cn

PHP:  class User {}
来源：http://hea.hnxiangtu.top

JS:   class User {}
来源：http://pfm.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://ckk.yuxming.cn

Java: class User {}
来源：http://ulb.zhixingplan.top

Go:   type User struct { Name string }
来源：http://fzl.0kj1m.cn

Ruby: class User; end
来源：http://yre.tarul.cn

C#:   class User {}
来源：http://ayb.dashuyun.cn

[G02] 构造函数
来源：http://psi.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://vmt.aizwys.cn

PHP:  public function __construct(public string $name) {}
来源：http://imx.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://suf.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://lqm.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://bpp.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bvd.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://xzw.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://zlf.gzhubu.top

[G03] 实例属性
来源：http://wkr.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://wrm.birdmap.top

PHP:  public string $name = "x";
来源：http://zuu.hnqzz.top

JS:   this.name = "x";
来源：http://vcq.zdqjudy.top

TS:   name: string = "x";
来源：http://wos.cashguo.top

Java: private String name;
来源：http://lbb.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://but.sjlbkw.cn

Ruby: @name = "x"
来源：http://vew.yangfankeji.com

C#:   public string Name { get; set; } = "x";
来源：http://eis.zycfv.cn

[G04] 定义方法
来源：http://ymm.sufxvd.cn

Py:   def greet(self): return self.name
来源：http://wjx.pycfn.com

PHP:  public function greet(): string { return $this->name; }
来源：http://sge.daria6918.cn

JS:   greet() { return this.name; }
来源：http://cse.zhixingplan.top

TS:   greet(): string { return this.name; }
来源：http://xjk.andypj.xyz

Java: String greet() { return name; }
来源：http://aiw.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vmr.tian-w.cn

Ruby: def greet; @name; end
来源：http://brp.tanke756.top

C#:   public string Greet() => Name;
来源：http://fdr.jlsjyb.cn

[G05] 继承
来源：http://blk.shzxlz.cn

Py:   class Admin(User): pass
来源：http://bkw.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://onq.yuanzhike.top

JS:   class Admin extends User {}
来源：http://chr.jlsjyb.cn

TS:   class Admin extends User {}
来源：http://vzo.yj20258888.top

Java: class Admin extends User {}
来源：http://qij.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jmr.smart0.xyz

Ruby: class Admin < User; end
来源：http://gqo.epnwcf.com

C#:   class Admin : User {}
来源：http://syw.gaohongyu789.top

[G06] 重写方法
来源：http://ozs.hywenlv.cn

Py:   def greet(self): return "admin"
来源：http://mxs.kuanghao11.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oyw.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://uuk.redwolf501.top

TS:   greet(): string { return "admin"; }
来源：http://aav.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://gon.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vha.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://kvg.ppjwa.cn

C#:   public override string Greet() => "admin";
来源：http://fob.yonumen.top

[G07] 调用父类方法
来源：http://crt.sjlbkw.cn

Py:   super().greet()
来源：http://gjo.zhiwuduotai.top

PHP:  parent::greet();
来源：http://qyq.shanyushiyangkeji.top

JS:   super.greet();
来源：http://axg.yangfankeji.com

TS:   super.greet();
来源：http://blt.sxryk.cn

Java: super.greet();
来源：http://rht.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dhw.hfpthk.cn


<!-- 参考信息 -->