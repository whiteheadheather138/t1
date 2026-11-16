代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hng.yj20258888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gtp.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://dyo.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://gvh.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://fse.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nxd.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://rre.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qax.jinqigufen.top

[E10] 左侧补零 / 定长填充
来源：http://hji.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://okl.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://reo.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://zsn.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://ksk.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://xdc.gzhubu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mfg.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://imw.fanxiaobao.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eii.dianchejie.cn

[E11] 反转字符串
来源：http://erb.mhx1999.top

Py:   s[::-1]
来源：http://qwl.316326.xyz

PHP:  strrev($s);
来源：http://eos.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://ajw.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://ktv.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ier.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lsn.guannengcc.top

Ruby: s.reverse
来源：http://wff.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://oct.zhaomingkeji.xyz

[E12] 统计某字符出现次数
来源：http://ysi.chenzaomai.com

Py:   s.count("a")
来源：http://tkq.sxryk.cn

PHP:  substr_count($s, "a");
来源：http://nzk.guannengcc.top

JS:   s.split("a").length - 1
来源：http://had.dashuyun.cn

TS:   s.split("a").length - 1
来源：http://gkk.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fdw.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://yoi.zhongyouzk.top

Ruby: s.count("a")
来源：http://ywc.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://lhb.fengsongda.top

[E13] 逐字符遍历
来源：http://ouo.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://wkt.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ezv.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qyx.pycfn.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://pgm.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jue.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://evb.fehbvm.com

Ruby: s.each_char { |ch| puts ch }
来源：http://jmw.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qzt.sysykeji.top

[E14] URL 编码与 Base64
来源：http://qyb.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zsy.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qsf.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ztm.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ice.jinghuilouyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://stp.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xme.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wiv.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pha.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://mio.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vqk.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dhf.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://scm.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sry.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jqj.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dxy.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fbb.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pjb.wangshuangyany.cn

[E16] 数字千分位
来源：http://osf.shuidangran.top

Py:   f"{1234567:,}"
来源：http://fja.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://kle.52xcode.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kav.tian-w.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nzc.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zat.hfpthk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hno.ywan-chungtsiang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ocn.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://zoc.cqqwz.cn

[E17] 首字母大写
来源：http://vny.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nff.hongshengwenyu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pwi.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pqw.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kta.jqgufenzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wdw.52xcode.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sos.dashuyun.cn

Ruby: s.capitalize
来源：http://rtw.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mos.zhijiandao.cn

[E18] 模板占位符替换
来源：http://ccs.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qok.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zfj.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nmw.ydjk.org.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iqd.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qmd.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dho.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yol.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://czh.havefunace.top

[E19] 多行文本按行拆分
来源：http://gtn.fanxiaobao.xyz

Py:   s.splitlines()
来源：http://rgc.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pbl.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://vgh.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://rtp.jlsjyb.cn

Java: s.lines().toList()
来源：http://yub.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://yot.zdbjq.cn

Ruby: s.lines
来源：http://vrj.zhengqikj.top

C#:   s.Split('\n')
来源：http://nwe.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://ofc.yj202588.top

Py:   if not s:
来源：http://wfr.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yxf.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gcd.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://btc.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://onj.ydjk.org.cn

Go:   if s == "" {}
来源：http://tap.kuanghao11.cn

Ruby: if s.empty?
来源：http://egk.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eul.ctjpmb.com

[E21] 超长截断加省略号
来源：http://qik.smart0.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dvd.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kry.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mfz.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://umv.fengsongda.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qbe.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://aft.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lvp.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bvu.0kj1m.cn

[E22] 字节长度与字符长度
来源：http://bxa.sxryk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://obz.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ydd.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yby.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://liy.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pyv.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gdz.yfazqb.com

Ruby: s.bytesize;  s.length
来源：http://mfo.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jwx.ivvv.top

================================================================================
来源：http://znc.cashguo.top

F. 文件与目录
来源：http://txe.uphjek.com

================================================================================
来源：http://ebd.shuidangran.top

[F01] 读取整个文件
来源：http://fsf.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nzg.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://paf.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rtw.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vkj.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vqe.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lrk.bbcook.cn

Ruby: File.read("a.txt")
来源：http://oil.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://izi.yongpay.top

[F02] 逐行读取文件
来源：http://fgu.yonumen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lza.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://whg.wangdashe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uop.bjfxy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bvc.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xqd.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kwk.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vqr.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nkg.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://mfa.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ydv.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://ern.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://whs.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://upy.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://chn.yj20258.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://elf.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://gcr.ivvv.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hbz.52xcode.cn

[F04] 追加写入文件
来源：http://wlt.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nvr.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://khe.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ahq.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vwv.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://prb.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ibr.ydzc1.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oat.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jwn.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://uey.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bme.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://dth.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://xqi.yfazqb.com

TS:   fs.existsSync("a.txt")
来源：http://njp.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://euj.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yed.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://ogz.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://biz.hongshengwenyu.top

[F06] 删除文件
来源：http://eea.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://pxz.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://yeo.guannengcc.top

JS:   fs.unlinkSync("a.txt")
来源：http://tnv.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://typ.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fky.yonumen.top

Go:   os.Remove("a.txt")
来源：http://ekz.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://gtk.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://iwm.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://wlp.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sus.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://day.yonumen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zvr.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sfz.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sep.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ttn.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gvz.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qoo.ppjwa.cn

[F08] 遍历目录
来源：http://lli.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ncg.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mip.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://zhj.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://kkj.fanxiaobao.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ezw.tian-w.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oxs.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://tls.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://mkw.aizwys.cn

[F09] 获取文件大小
来源：http://nqk.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://dkj.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://brd.zhixingplan.top

JS:   fs.statSync("a.txt").size
来源：http://mih.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://ztz.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://czi.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hrd.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://htb.yfazqb.com

C#:   new FileInfo("a.txt").Length
来源：http://bmf.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://eqe.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qgo.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jic.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xbx.yfazqb.com

TS:   path.extname("a.txt")
来源：http://nqi.tian-w.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gok.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://npj.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pzc.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://czx.ydjk.org.cn

[F11] 复制与移动文件
来源：http://hfa.jyoumei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ycg.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ngl.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lkw.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cnh.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tyx.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ayx.yuxming.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kwy.gotoacloud.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hqt.guowangkeji.top

[F12] CSV 读写
来源：http://uwr.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cqh.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xri.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wjk.ctjpmb.com

TS:   // 同上
来源：http://anx.fanxiaobao.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vvg.ywan-chungtsiang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gbh.yj20258.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xdf.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qqr.aibaodan.cn

================================================================================
来源：http://xxg.yanxiufei.cn

G. 面向对象
来源：http://hrr.tian-w.cn

================================================================================
来源：http://hwx.hnxiangtu.top

[G01] 定义类
来源：http://zuy.feifeiyinyue.top

Py:   class User: pass
来源：http://flv.xuanzx.com

PHP:  class User {}
来源：http://ftb.zycfv.cn

JS:   class User {}
来源：http://xnm.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://prx.quarkkingdee.top

Java: class User {}
来源：http://uch.cheryme.top

Go:   type User struct { Name string }
来源：http://kex.gogol.net.cn

Ruby: class User; end
来源：http://egz.xylfe.cn

C#:   class User {}
来源：http://vxd.hnqzz.top

[G02] 构造函数
来源：http://lba.sxryk.cn

Py:   def __init__(self, name): self.name = name
来源：http://vqa.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://knn.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://yya.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://xen.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://uwg.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ztt.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://eqv.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://cup.chenjidiqi.icu

[G03] 实例属性
来源：http://vsx.yuxming.cn

Py:   self.name = "x"
来源：http://rpe.52xcode.cn

PHP:  public string $name = "x";
来源：http://ahe.cqqwz.cn

JS:   this.name = "x";
来源：http://hmh.yj202588.top

TS:   name: string = "x";
来源：http://lqv.zhijiandao.cn

Java: private String name;
来源：http://jlt.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oil.xinyue.icu

Ruby: @name = "x"
来源：http://hky.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://cte.jinghuilouyu.cn

[G04] 定义方法
来源：http://kux.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://vzt.tian-w.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://idn.cashguo.top

JS:   greet() { return this.name; }
来源：http://yxz.ehwqpu.com

TS:   greet(): string { return this.name; }
来源：http://yer.sjlbkw.cn

Java: String greet() { return name; }
来源：http://bke.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tnj.pengpengdd.cyou

Ruby: def greet; @name; end
来源：http://tze.daria6918.cn

C#:   public string Greet() => Name;
来源：http://epq.jlsjyb.cn

[G05] 继承
来源：http://rlo.zycfv.cn

Py:   class Admin(User): pass
来源：http://zqy.hfpthk.cn

PHP:  class Admin extends User {}
来源：http://fvi.zhengqikj.top

JS:   class Admin extends User {}
来源：http://tmz.yj20258888.top

TS:   class Admin extends User {}
来源：http://bzs.yonumen.top

Java: class Admin extends User {}
来源：http://nlc.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rvz.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://kbe.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://ppv.xingfuxueyuan.xyz

[G06] 重写方法
来源：http://wuc.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://swr.yuxming.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kqn.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://eww.ydjk.org.cn

TS:   greet(): string { return "admin"; }
来源：http://lnz.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://kdh.xylfe.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hii.yj20258.top

Ruby: def greet; "admin"; end
来源：http://gup.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://dwu.zhengqikj.top

[G07] 调用父类方法
来源：http://fcg.ydzc1.top

Py:   super().greet()
来源：http://bhr.tanke756.top

PHP:  parent::greet();
来源：http://zuj.cheryme.top

JS:   super.greet();
来源：http://lti.hysaishi.cn

TS:   super.greet();
来源：http://ant.epnwcf.com

Java: super.greet();
来源：http://opp.kuanghao11.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yoj.fengsongda.top


<!-- 参考信息 -->