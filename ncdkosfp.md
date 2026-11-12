代发 wailian999

Go:   strings.Join(items, ",")
来源：http://nqx.jyoumei.cn

Ruby: items.join(",")
来源：http://hql.yj20258888.top

C#:   string.Join(",", items)
来源：http://sqo.gzhubu.top

[E09] 去除所有空白字符
来源：http://hoa.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pgi.quarkkingdee.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mfu.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://ssl.ydjk.org.cn

TS:   s.replace(/\s+/g, "")
来源：http://fzj.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://fws.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://awg.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qpj.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nrq.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://bsx.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://utx.yj202588.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lmy.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://wek.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://bhc.shanyushiyangkeji.top

Java: String.format("%03d", 7)
来源：http://uda.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wyw.hysaishi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cqn.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jec.yj202588.top

[E11] 反转字符串
来源：http://lgq.jlsjyb.cn

Py:   s[::-1]
来源：http://anv.hnqzz.top

PHP:  strrev($s);
来源：http://yhu.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://qra.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://idz.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jfa.cqqwz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ifr.jyoumei.cn

Ruby: s.reverse
来源：http://jqz.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://ogt.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://jex.sysykeji.top

Py:   s.count("a")
来源：http://yyl.ywan-chungtsiang.top

PHP:  substr_count($s, "a");
来源：http://ceu.tarul.cn

JS:   s.split("a").length - 1
来源：http://tpr.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://bts.snrcjt.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hvt.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://woo.ywan-chungtsiang.top

Ruby: s.count("a")
来源：http://ozs.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://uyg.zhoulong.xyz

[E13] 逐字符遍历
来源：http://rqy.c1oappe.top

Py:   for ch in s: print(ch)
来源：http://cmf.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://unv.pengpengdd.cyou

JS:   for (const ch of s) { console.log(ch); }
来源：http://cai.yfazqb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://lxq.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tfz.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zkw.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wkn.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://upn.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://grs.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hay.sysykeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kbb.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://alp.316326.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qfq.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gxy.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dur.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vpv.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bmv.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://qyw.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://kjc.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dho.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mrz.jinghuilouyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lqd.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hhz.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gzy.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://anw.yj20258888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yci.yj202588.top

[E16] 数字千分位
来源：http://zko.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://qqm.yj20258.top

PHP:  number_format(1234567);
来源：http://wix.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://axk.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qnt.pycfn.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cpg.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sid.xylfe.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dsz.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://zmb.fengsongda.top

[E17] 首字母大写
来源：http://kzs.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cca.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lbe.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sdz.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oav.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://edr.dianchejie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tmt.vehdjk.com

Ruby: s.capitalize
来源：http://tul.shuidangran.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vvh.yangfankeji.com

[E18] 模板占位符替换
来源：http://hwg.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qcn.bjfxy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dcp.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cmc.guannengcc.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qje.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fye.epnwcf.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sbj.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gli.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rua.yuxming.cn

[E19] 多行文本按行拆分
来源：http://bnm.yj20258888.top

Py:   s.splitlines()
来源：http://dro.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dzo.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://cry.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://odn.aizwys.cn

Java: s.lines().toList()
来源：http://dng.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://goa.zhengqikj.top

Ruby: s.lines
来源：http://kna.ivvv.top

C#:   s.Split('\n')
来源：http://rro.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://nwd.316326.xyz

Py:   if not s:
来源：http://amg.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ywh.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hpl.redwolf501.top

TS:   if (s === "") {}
来源：http://bjy.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://iov.0kj1m.cn

Go:   if s == "" {}
来源：http://xkh.zhiwuduotai.top

Ruby: if s.empty?
来源：http://nll.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bib.yj20258888.top

[E21] 超长截断加省略号
来源：http://aea.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://flt.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jym.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nch.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ssk.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://grv.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://shw.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kem.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qgz.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://gko.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://boo.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ppv.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iyu.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bws.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mcr.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kwj.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://fbs.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ojd.fanxiaobao.xyz

================================================================================
来源：http://nnd.shuidangran.top

F. 文件与目录
来源：http://tbp.kuanghao11.cn

================================================================================
来源：http://ukd.uphjek.com

[F01] 读取整个文件
来源：http://vkx.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yho.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://hst.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kfb.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wem.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://qzj.zhaomingkeji.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://psu.meibo888.top

Ruby: File.read("a.txt")
来源：http://csa.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://rps.bbcook.cn

[F02] 逐行读取文件
来源：http://dyv.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uzz.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bmr.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xyu.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pjr.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tka.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://czs.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eji.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hdd.vehdjk.com

[F03] 写入文件（覆盖）
来源：http://qsz.shuidangran.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://odc.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://wgk.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lrj.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lpx.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hyf.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hjw.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://faf.fehbvm.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aki.zhoulong.xyz

[F04] 追加写入文件
来源：http://gqz.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://laq.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eqx.52xcode.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ysm.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vmf.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vsj.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://okn.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ndi.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wkb.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://ojk.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dfh.hywenlv.cn

PHP:  file_exists("a.txt");
来源：http://rdb.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://jqs.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://cwv.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dhz.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cpv.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://juj.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://qoj.xuetiantiany.cn

[F06] 删除文件
来源：http://iup.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://vxk.havefunace.top

PHP:  unlink("a.txt");
来源：http://zpb.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://ibm.yongpay.top

TS:   fs.unlinkSync("a.txt")
来源：http://pjt.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sng.tanke756.top

Go:   os.Remove("a.txt")
来源：http://opl.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://sjd.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://axc.yueranfly.top

[F07] 创建目录（含多级）
来源：http://ptr.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ejs.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://awp.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wbg.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nml.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sfp.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gfz.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pdb.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cqn.smart0.xyz

[F08] 遍历目录
来源：http://goq.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rzp.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ixy.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://tpt.vqdsnc.cn

TS:   fs.readdirSync("dir")
来源：http://jpc.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://raa.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zbe.sweek.top

Ruby: Dir.children("dir")
来源：http://xli.vqdsnc.cn

C#:   Directory.GetFiles("dir")
来源：http://ckf.cqqwz.cn

[F09] 获取文件大小
来源：http://lda.bjfxy.top

Py:   os.path.getsize("a.txt")
来源：http://qkr.aizwys.cn

PHP:  filesize("a.txt");
来源：http://zrb.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://qjq.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://cpg.xingfuxueyuan.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://qht.yangfankeji.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://duq.zhoulong.xyz

Ruby: File.size("a.txt")
来源：http://pth.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://gtc.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://gsz.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://skk.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yqj.yongpay.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hov.meibo888.top

TS:   path.extname("a.txt")
来源：http://gtu.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xud.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pvr.shangyingyoupin.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://npy.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jkl.sweek.top

[F11] 复制与移动文件
来源：http://ikt.jyoumei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bwd.cucudq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://miy.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eqw.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fza.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mmd.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hzg.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mrc.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://whm.sjlbkw.cn

[F12] CSV 读写
来源：http://eex.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dge.chenlongwang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ffw.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kyy.dashuyun.cn

TS:   // 同上
来源：http://uhq.hysaishi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://doj.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://smz.hnxiangtu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mnc.fanxiaobao.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://ykm.xuetiantiany.cn

================================================================================
来源：http://jpo.fehbvm.com

G. 面向对象
来源：http://nki.hesvh.cn

================================================================================
来源：http://mrd.daxiang520.top

[G01] 定义类
来源：http://akd.meibo888.top

Py:   class User: pass
来源：http://arm.jinqigfzy.top

PHP:  class User {}
来源：http://caf.guowangkeji.top

JS:   class User {}
来源：http://jxq.hysaishi.cn

TS:   class User { name: string = ""; }
来源：http://dfc.yanxiufei.cn

Java: class User {}
来源：http://lcv.zycfv.cn

Go:   type User struct { Name string }
来源：http://glk.yuxming.cn

Ruby: class User; end
来源：http://qly.yongpay.top

C#:   class User {}
来源：http://imd.chenjidiqi.icu

[G02] 构造函数
来源：http://nvp.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://amk.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://ece.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://zrd.epnwcf.com

TS:   constructor(public name: string) {}
来源：http://xcf.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://szo.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bsy.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://byg.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://euy.jiagoushi.top

[G03] 实例属性
来源：http://ikx.hfpthk.cn

Py:   self.name = "x"
来源：http://zhz.yj20258.top

PHP:  public string $name = "x";
来源：http://pmu.jinqigfzy.top

JS:   this.name = "x";
来源：http://hfr.sweek.top

TS:   name: string = "x";
来源：http://rrp.xylfe.cn

Java: private String name;
来源：http://qht.pycfn.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nvd.chenlongwang.top

Ruby: @name = "x"
来源：http://zkk.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://eze.xylfe.cn

[G04] 定义方法
来源：http://fth.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://dhp.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://vrl.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://hja.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://qmw.cucudq.cn

Java: String greet() { return name; }
来源：http://ekg.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pmd.tanke756.top

Ruby: def greet; @name; end
来源：http://man.ydzc1.top

C#:   public string Greet() => Name;
来源：http://now.gzhubu.top

[G05] 继承
来源：http://uwy.yueranfly.top

Py:   class Admin(User): pass
来源：http://ugp.hywenlv.cn

PHP:  class Admin extends User {}
来源：http://ixg.cdnleiting.top

JS:   class Admin extends User {}
来源：http://art.sysykeji.top

TS:   class Admin extends User {}
来源：http://wnf.zhongyouzk.top

Java: class Admin extends User {}
来源：http://vaj.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mle.fktsv.cn

Ruby: class Admin < User; end
来源：http://cey.kuanghao11.cn

C#:   class Admin : User {}
来源：http://nrs.andypj.xyz

[G06] 重写方法
来源：http://sow.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://vxu.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lsc.zhengqikj.top

JS:   greet() { return "admin"; }
来源：http://huf.hongshengwenyu.top

TS:   greet(): string { return "admin"; }
来源：http://jdz.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://lzu.hnqzz.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bjd.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://mek.havefunace.top

C#:   public override string Greet() => "admin";
来源：http://fxi.zycfv.cn

[G07] 调用父类方法
来源：http://ehh.jianghu66.top

Py:   super().greet()
来源：http://xoj.sxryk.cn

PHP:  parent::greet();
来源：http://rbw.hesvh.cn


<!-- 参考信息 -->