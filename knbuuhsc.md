代发 wailian999

Go:   strings.Join(items, ",")
来源：http://ctr.fehbvm.com

Ruby: items.join(",")
来源：http://jgl.epnwcf.com

C#:   string.Join(",", items)
来源：http://jlu.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://hbi.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qck.iojbl.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hhk.bjfxy.top

JS:   s.replace(/\s+/g, "")
来源：http://lil.zdbjq.cn

TS:   s.replace(/\s+/g, "")
来源：http://ixc.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://gsc.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xdx.zdbjq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wva.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://git.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://mpk.shangyingyoupin.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fvw.gaohongyu789.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qlc.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://itd.sysykeji.top

TS:   "7".padStart(3, "0")
来源：http://spe.c1oappe.top

Java: String.format("%03d", 7)
来源：http://dhr.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mjt.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iyv.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://btk.jqgfzy.top

[E11] 反转字符串
来源：http://jlr.chenzaomai.com

Py:   s[::-1]
来源：http://czf.aizwys.cn

PHP:  strrev($s);
来源：http://nlo.yvedp.cn

JS:   [...s].reverse().join("")
来源：http://lma.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://dzj.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hbn.yuxming.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://plv.sxryk.cn

Ruby: s.reverse
来源：http://coo.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://alv.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://bdw.tanke756.top

Py:   s.count("a")
来源：http://ywm.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://lau.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://lfd.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://zec.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://azw.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://lmx.fengsongda.top

Ruby: s.count("a")
来源：http://pvv.cdnleiting.top

C#:   s.Count(c => c == 'a')
来源：http://gju.guannengcc.top

[E13] 逐字符遍历
来源：http://vmj.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://ajn.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vaq.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fsm.gotoacloud.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pzs.hongshengwenyu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qhn.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zse.havefunace.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rkc.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wrt.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://cyf.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ysp.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://hnt.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iys.daria6918.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bft.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aid.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pgv.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hkz.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lcw.andypj.xyz

[E15] HTML 转义 / 反转义
来源：http://rvc.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://oig.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nfo.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ufw.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rfw.yuanzhike.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pkv.yonumen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bsm.nanxinkj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xhj.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bls.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://dpr.fengsongda.top

Py:   f"{1234567:,}"
来源：http://dkv.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://mgm.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://anq.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ymm.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pwq.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mob.havefunace.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wkj.yj20258.top

C#:   1234567.ToString("N0")
来源：http://vnc.ehwqpu.com

[E17] 首字母大写
来源：http://suh.jinghuilouyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vct.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://flv.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nbp.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fqv.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://now.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gak.jianghu66.top

Ruby: s.capitalize
来源：http://hqu.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fiz.c1oappe.top

[E18] 模板占位符替换
来源：http://zep.chenjidiqi.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eta.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jge.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uek.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jjd.fzhhl.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xre.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aey.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://grk.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rdl.yj20258888.top

[E19] 多行文本按行拆分
来源：http://ncl.wangshuangyany.cn

Py:   s.splitlines()
来源：http://yuh.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hua.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://vnq.yanxiufei.cn

TS:   s.split(/\r?\n/)
来源：http://lcd.52xcode.cn

Java: s.lines().toList()
来源：http://lpo.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://oce.bjfxy.top

Ruby: s.lines
来源：http://fvy.daxiang520.top

C#:   s.Split('\n')
来源：http://bow.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://rxf.jqgufenzy.top

Py:   if not s:
来源：http://xyy.fktsv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lfg.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rwu.ydjk.org.cn

TS:   if (s === "") {}
来源：http://mgb.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://xpi.yvedp.cn

Go:   if s == "" {}
来源：http://wvx.ybcxt.top

Ruby: if s.empty?
来源：http://tka.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nqr.wangdashe.top

[E21] 超长截断加省略号
来源：http://tag.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vtr.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://adr.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hox.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jbr.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dba.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://glu.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nav.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://maa.xylfe.cn

[E22] 字节长度与字符长度
来源：http://swd.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mqy.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iov.yanxiufei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://laa.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://don.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zav.316326.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jhq.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://xja.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mtk.hnqzz.top

================================================================================
来源：http://wso.vqdsnc.cn

F. 文件与目录
来源：http://ldq.tanke756.top

================================================================================
来源：http://uqa.yj20258888.top

[F01] 读取整个文件
来源：http://lna.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qpt.jqgfzy.top

PHP:  file_get_contents("a.txt");
来源：http://bzc.redwolf501.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rfy.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://skx.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zpp.xinyue.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ezq.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://bml.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://ioq.chenlongwang.top

[F02] 逐行读取文件
来源：http://xpb.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cwz.cheryme.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pad.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hbr.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ilr.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://how.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jpt.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sfk.tanke756.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fff.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://omr.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kyy.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nfe.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kyt.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hjp.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iye.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://auz.jianghu66.top

Ruby: File.write("a.txt", "hi")
来源：http://kta.sweek.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mft.zhoulong.xyz

[F04] 追加写入文件
来源：http://xph.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pnq.hfpthk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ypy.pengpengdd.cyou

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vso.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oao.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://add.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fwf.yj202588.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tnr.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mdx.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://yld.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sys.yj202588.top

PHP:  file_exists("a.txt");
来源：http://vmq.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://vbj.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://ajf.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://flu.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rlc.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://ubx.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://dbc.feifeiyinyue.top

[F06] 删除文件
来源：http://bzq.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://xoc.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://qhd.sweek.top

JS:   fs.unlinkSync("a.txt")
来源：http://bgk.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://wmz.pycfn.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://htx.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://jne.hnqzz.top

Ruby: File.delete("a.txt")
来源：http://hqh.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://lde.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://kog.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mpw.tanke756.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qvr.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ifm.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://spv.sweek.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cpp.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qcb.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wwp.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xgs.xuanzx.com

[F08] 遍历目录
来源：http://wah.aibaodan.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hvg.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ogn.snrcjt.cn

JS:   fs.readdirSync("dir")
来源：http://tmm.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://onp.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cls.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://smz.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://mrd.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://kvd.feifeiyinyue.top

[F09] 获取文件大小
来源：http://skk.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://ykf.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://sur.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://cas.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://chz.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://plf.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zxi.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://ghk.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://vzg.hcnkem.com

[F10] 取文件扩展名 / 文件名
来源：http://ivt.zdqjudy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xtq.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cfy.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bzs.jinqigufen.top

TS:   path.extname("a.txt")
来源：http://jzv.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xpk.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vuu.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yry.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dcm.chenzaomai.com

[F11] 复制与移动文件
来源：http://qxv.fanxiaobao.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uer.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kau.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tph.shuidangran.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mzw.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lcy.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uod.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bpo.gogol.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jew.ppjwa.cn

[F12] CSV 读写
来源：http://axs.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kse.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rdc.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ivs.ctjpmb.com

TS:   // 同上
来源：http://lni.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bwk.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bza.yj20258.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pir.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jim.jinghuilouyu.cn

================================================================================
来源：http://hxd.zhaomingkeji.xyz

G. 面向对象
来源：http://owa.ivvv.top

================================================================================
来源：http://clb.yfazqb.com

[G01] 定义类
来源：http://scq.aizwys.cn

Py:   class User: pass
来源：http://nhb.snrcjt.cn

PHP:  class User {}
来源：http://fic.xziqi.cn

JS:   class User {}
来源：http://kfs.sweek.top

TS:   class User { name: string = ""; }
来源：http://xef.cucudq.cn

Java: class User {}
来源：http://dit.chenjidiqi.icu

Go:   type User struct { Name string }
来源：http://zlm.jiagoushi.top

Ruby: class User; end
来源：http://vrm.andypj.xyz

C#:   class User {}
来源：http://yyh.wangdashe.top

[G02] 构造函数
来源：http://dse.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://cih.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://xai.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://ldx.yonumen.top

TS:   constructor(public name: string) {}
来源：http://jie.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://erw.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wmn.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://duj.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://dlj.316326.xyz

[G03] 实例属性
来源：http://szo.nwbrower.top

Py:   self.name = "x"
来源：http://ntc.cdnleiting.top

PHP:  public string $name = "x";
来源：http://alk.xingfuxueyuan.xyz

JS:   this.name = "x";
来源：http://vgl.meibo888.top

TS:   name: string = "x";
来源：http://iju.shuidangran.top

Java: private String name;
来源：http://mhb.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vsa.cqqwz.cn

Ruby: @name = "x"
来源：http://qvv.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://mqu.9152youxi.cn

[G04] 定义方法
来源：http://qlh.aibaodan.cn

Py:   def greet(self): return self.name
来源：http://ztr.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://use.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://frb.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://ecx.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://irk.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://unu.feifeiyinyue.top

Ruby: def greet; @name; end
来源：http://jkc.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://eog.cashguo.top

[G05] 继承
来源：http://cmn.gogol.net.cn

Py:   class Admin(User): pass
来源：http://yud.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://dwq.c1oappe.top

JS:   class Admin extends User {}
来源：http://slf.hysaishi.cn

TS:   class Admin extends User {}
来源：http://htj.fktsv.cn

Java: class Admin extends User {}
来源：http://byo.zhongyouzk.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wpg.zdqjudy.top

Ruby: class Admin < User; end
来源：http://lto.xinyue.icu

C#:   class Admin : User {}
来源：http://dat.zhaomingkeji.xyz

[G06] 重写方法
来源：http://mwg.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://ifa.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://icr.jqgfzy.top

JS:   greet() { return "admin"; }
来源：http://jty.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://trq.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://kdm.sxryk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://egl.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://lit.andypj.xyz

C#:   public override string Greet() => "admin";
来源：http://eul.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://uqf.zycfv.cn

Py:   super().greet()
来源：http://ikm.wangdashe.top

PHP:  parent::greet();
来源：http://iqh.zdbjq.cn


<!-- 参考信息 -->