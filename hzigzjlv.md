代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hxd.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bpi.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://fgt.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://riq.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://gzq.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jmw.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://lth.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://awe.yongpay.top

[E10] 左侧补零 / 定长填充
来源：http://wox.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vvb.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ccc.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://gpd.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://rty.daxiang520.top

Java: String.format("%03d", 7)
来源：http://umz.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vcs.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zkz.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tmh.ctjpmb.com

[E11] 反转字符串
来源：http://cit.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://any.zhongyouzk.top

PHP:  strrev($s);
来源：http://sup.ppjwa.cn

JS:   [...s].reverse().join("")
来源：http://fgc.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://viw.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lbr.xuetiantiany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hbr.zhengqikj.top

Ruby: s.reverse
来源：http://jyf.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://pku.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://dld.yangfankeji.com

Py:   s.count("a")
来源：http://siw.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://foa.zhiwuduotai.top

JS:   s.split("a").length - 1
来源：http://qjo.jyoumei.cn

TS:   s.split("a").length - 1
来源：http://yzz.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://itn.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://mvs.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://ifu.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://yld.epnwcf.com

[E13] 逐字符遍历
来源：http://dbf.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://vdp.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://beu.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gzu.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ens.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gxa.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mze.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://lxf.jinghuilouyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lap.iojbl.cn

[E14] URL 编码与 Base64
来源：http://juu.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://txc.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kzy.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cqr.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nrw.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wcw.kuanghao11.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qpw.jyoumei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pda.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ezy.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://szp.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ugf.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://twe.gotoacloud.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cvd.hnxiangtu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://abs.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sko.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ydq.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ips.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://omx.jqgfzy.top

[E16] 数字千分位
来源：http://vjo.birdmap.top

Py:   f"{1234567:,}"
来源：http://jvb.cdnleiting.top

PHP:  number_format(1234567);
来源：http://ngk.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cxj.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wtc.xingfuxueyuan.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aiu.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dfi.fktsv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ihz.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://lnm.yj20258.top

[E17] 首字母大写
来源：http://rsh.hnxiangtu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aqj.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://czc.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://map.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vbd.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sti.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://asw.sweek.top

Ruby: s.capitalize
来源：http://qms.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rmx.zhixingplan.top

[E18] 模板占位符替换
来源：http://oqi.yongpay.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yjf.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ovn.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lgo.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oty.yj20258.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xuj.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pjc.yfazqb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://beb.hfpthk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qsf.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://igx.cashguo.top

Py:   s.splitlines()
来源：http://qfn.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://apv.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://wbl.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://zxp.yj202588.top

Java: s.lines().toList()
来源：http://zcb.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://stz.tianlin.xyz

Ruby: s.lines
来源：http://gcf.jlsjyb.cn

C#:   s.Split('\n')
来源：http://xqv.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://imo.xinyue.icu

Py:   if not s:
来源：http://ypj.feifeiyinyue.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hvd.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ezl.zhijiandao.cn

TS:   if (s === "") {}
来源：http://sxz.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://stw.jianghu66.top

Go:   if s == "" {}
来源：http://ewj.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://dfh.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vln.sxryk.cn

[E21] 超长截断加省略号
来源：http://yob.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://duw.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mda.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kln.ehwqpu.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ztf.sjlbkw.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vqa.shanyushiyangtech.top

Go:   // 按 rune 判断长度后截断
来源：http://slx.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nvr.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://env.hesvh.cn

[E22] 字节长度与字符长度
来源：http://zdj.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tqw.guannengcc.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ucq.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nxg.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://umq.yongpay.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fgj.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ypb.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://bao.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cqs.jiagoushi.top

================================================================================
来源：http://isd.hesvh.cn

F. 文件与目录
来源：http://usd.sxryk.cn

================================================================================
来源：http://rix.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://fsx.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nve.zycfv.cn

PHP:  file_get_contents("a.txt");
来源：http://wyv.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lkd.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://twb.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dml.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zcp.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://ihw.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://lvl.yfazqb.com

[F02] 逐行读取文件
来源：http://sgx.jinqigfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lxg.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wum.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dmj.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wun.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://twl.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://urj.yvedp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bvn.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fps.ivvv.top

[F03] 写入文件（覆盖）
来源：http://sub.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fvu.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ijk.wangdashe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mlw.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qxj.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eeh.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://piy.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://pri.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ybi.hongshengwenyu.top

[F04] 追加写入文件
来源：http://bqc.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ljo.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rci.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tpu.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gfn.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vxx.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fvp.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bem.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jdw.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://eib.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rht.pycfn.com

PHP:  file_exists("a.txt");
来源：http://zbm.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://bhj.hesvh.cn

TS:   fs.existsSync("a.txt")
来源：http://duz.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ugj.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jzj.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://bhr.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://vgn.shanyushiyangtech.top

[F06] 删除文件
来源：http://ftp.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://mwm.52xcode.cn

PHP:  unlink("a.txt");
来源：http://bpq.birdmap.top

JS:   fs.unlinkSync("a.txt")
来源：http://pav.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://njz.chenlongwang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nzt.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://xuo.pycfn.com

Ruby: File.delete("a.txt")
来源：http://yfx.fengsongda.top

C#:   File.Delete("a.txt");
来源：http://xme.andypj.xyz

[F07] 创建目录（含多级）
来源：http://knl.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://trv.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vah.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lhh.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lgo.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://euf.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ovf.hongshengwenyu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mml.cheryme.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jae.vehdjk.com

[F08] 遍历目录
来源：http://cfm.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wep.yuxming.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://anv.jlsjyb.cn

JS:   fs.readdirSync("dir")
来源：http://wvu.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://nzf.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mgr.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gwm.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://ild.daxiang520.top

C#:   Directory.GetFiles("dir")
来源：http://ngl.aibaodan.cn

[F09] 获取文件大小
来源：http://qjt.vqdsnc.cn

Py:   os.path.getsize("a.txt")
来源：http://nsq.sweek.top

PHP:  filesize("a.txt");
来源：http://ayh.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://euv.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://qyh.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://fag.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pjv.xylfe.cn

Ruby: File.size("a.txt")
来源：http://gbo.316326.xyz

C#:   new FileInfo("a.txt").Length
来源：http://vub.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://vgb.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dsm.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dqc.yvedp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tof.yvedp.cn

TS:   path.extname("a.txt")
来源：http://skt.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jtp.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pkx.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wsz.vehdjk.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uzc.fehbvm.com

[F11] 复制与移动文件
来源：http://oct.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ole.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zcf.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iua.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qou.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kiy.jiagoushi.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ren.xingfuxueyuan.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qvj.havefunace.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ynu.guowangkeji.top

[F12] CSV 读写
来源：http://ydq.nanxinkj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eci.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bzr.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pxf.bjfxy.top

TS:   // 同上
来源：http://ufx.jyoumei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qzg.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lov.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://thz.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kfe.jiagoushi.top

================================================================================
来源：http://onc.nanxinkj.top

G. 面向对象
来源：http://kcu.chenzaomai.com

================================================================================
来源：http://ebk.zhiwuduotai.top

[G01] 定义类
来源：http://jfq.jyoumei.cn

Py:   class User: pass
来源：http://kac.havefunace.top

PHP:  class User {}
来源：http://cjr.shzxlz.cn

JS:   class User {}
来源：http://nmp.meibo888.top

TS:   class User { name: string = ""; }
来源：http://cgo.yonumen.top

Java: class User {}
来源：http://nkb.nwbrower.top

Go:   type User struct { Name string }
来源：http://ppc.hongshengwenyu.top

Ruby: class User; end
来源：http://iho.jyoumei.cn

C#:   class User {}
来源：http://emp.shanyushiyangtech.top

[G02] 构造函数
来源：http://fdr.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://vap.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://woe.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://frk.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://old.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://xol.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bsr.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://vax.316326.xyz

C#:   public User(string name) { Name = name; }
来源：http://soq.yanxiufei.cn

[G03] 实例属性
来源：http://tmn.chenlongwang.top

Py:   self.name = "x"
来源：http://zjk.shanyushiyangkeji.top

PHP:  public string $name = "x";
来源：http://twm.gotoacloud.top

JS:   this.name = "x";
来源：http://dhn.ppjwa.cn

TS:   name: string = "x";
来源：http://mvo.cheryme.top

Java: private String name;
来源：http://zzc.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tkh.havefunace.top

Ruby: @name = "x"
来源：http://llr.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://eys.jlsjyb.cn

[G04] 定义方法
来源：http://kbh.xziqi.cn

Py:   def greet(self): return self.name
来源：http://ooy.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://thj.yj20258888.top

JS:   greet() { return this.name; }
来源：http://gmr.hammf.cn

TS:   greet(): string { return this.name; }
来源：http://fkv.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://nja.jianghu66.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cmt.dianchejie.cn

Ruby: def greet; @name; end
来源：http://jma.cheryme.top

C#:   public string Greet() => Name;
来源：http://laf.yangfankeji.com

[G05] 继承
来源：http://oho.dianchejie.cn

Py:   class Admin(User): pass
来源：http://emn.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://ieg.fanxiaobao.xyz

JS:   class Admin extends User {}
来源：http://oru.yuanzhike.top

TS:   class Admin extends User {}
来源：http://ptf.redwolf501.top

Java: class Admin extends User {}
来源：http://fsk.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bqw.yj202588.top

Ruby: class Admin < User; end
来源：http://wqz.tarul.cn

C#:   class Admin : User {}
来源：http://fgz.fzhhl.top

[G06] 重写方法
来源：http://bxz.tarul.cn

Py:   def greet(self): return "admin"
来源：http://jcy.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://qyx.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://qzd.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://mga.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://wek.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zgf.hywenlv.cn

Ruby: def greet; "admin"; end
来源：http://wqf.redwolf501.top

C#:   public override string Greet() => "admin";
来源：http://low.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://gaj.shangyingyoupin.top

Py:   super().greet()
来源：http://glr.ehwqpu.com

PHP:  parent::greet();
来源：http://utw.gzhubu.top

JS:   super.greet();
来源：http://uve.yongpay.top

TS:   super.greet();
来源：http://ugt.zhixingplan.top

Java: super.greet();
来源：http://svm.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rpz.yuanzhike.top


<!-- 参考信息 -->