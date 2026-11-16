代发 wailian999

Go:   strings.Join(items, ",")
来源：http://uqg.zhixingplan.top

Ruby: items.join(",")
来源：http://oph.svipenyu.cn

C#:   string.Join(",", items)
来源：http://lyx.meibo888.top

[E09] 去除所有空白字符
来源：http://bwg.meibo888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://inu.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qce.ydjk.org.cn

JS:   s.replace(/\s+/g, "")
来源：http://fwm.hcnkem.com

TS:   s.replace(/\s+/g, "")
来源：http://kxw.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://vju.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ceb.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://xtp.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://umg.ydzc1.top

[E10] 左侧补零 / 定长填充
来源：http://stl.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dtn.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nxz.ybcxt.top

JS:   "7".padStart(3, "0")
来源：http://sza.ybcxt.top

TS:   "7".padStart(3, "0")
来源：http://ztc.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://glh.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mam.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jar.daxiang520.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vqh.0kj1m.cn

[E11] 反转字符串
来源：http://zdh.dashuyun.cn

Py:   s[::-1]
来源：http://sbz.yueranfly.top

PHP:  strrev($s);
来源：http://pjg.nanxinkj.top

JS:   [...s].reverse().join("")
来源：http://cjn.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://paq.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gyu.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rdu.jqgfzy.top

Ruby: s.reverse
来源：http://xvq.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://krb.fktsv.cn

[E12] 统计某字符出现次数
来源：http://zib.dianchejie.cn

Py:   s.count("a")
来源：http://jlz.zhengqikj.top

PHP:  substr_count($s, "a");
来源：http://egy.daxiang520.top

JS:   s.split("a").length - 1
来源：http://bju.tian-w.cn

TS:   s.split("a").length - 1
来源：http://noj.xylfe.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hdl.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://nic.jiagoushi.top

Ruby: s.count("a")
来源：http://ecz.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://nug.zhengqikj.top

[E13] 逐字符遍历
来源：http://lkb.meibo888.top

Py:   for ch in s: print(ch)
来源：http://fnh.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fae.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hsh.hammf.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://faf.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cwc.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jix.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ddz.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iml.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://khs.aizwys.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dyb.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bsn.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wzq.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ftq.sufxvd.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rly.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hsw.yj20258.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qcx.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dtb.sysykeji.top

[E15] HTML 转义 / 反转义
来源：http://uhp.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jst.hfpthk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fgw.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tod.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rbs.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xtw.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ssa.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kms.52xcode.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://chr.yfazqb.com

[E16] 数字千分位
来源：http://cyt.52xcode.cn

Py:   f"{1234567:,}"
来源：http://eez.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://uoo.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://whg.nanxuanxn.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jtt.nwbrower.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xpz.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ccs.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dgd.havefunace.top

C#:   1234567.ToString("N0")
来源：http://qkx.jiagoushi.top

[E17] 首字母大写
来源：http://vkc.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vdx.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qpq.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bhs.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ecp.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pwt.wangshuangyany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zra.cucudq.cn

Ruby: s.capitalize
来源：http://udd.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cxa.sxryk.cn

[E18] 模板占位符替换
来源：http://lkf.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ghr.hongshengwenyu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gdd.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ryr.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://pmk.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zdd.ppjwa.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yyj.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lsc.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kvk.xinyue.icu

[E19] 多行文本按行拆分
来源：http://lkd.zhiwuduotai.top

Py:   s.splitlines()
来源：http://hns.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://odo.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://bqc.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://ryt.sweek.top

Java: s.lines().toList()
来源：http://hvq.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://cem.tarul.cn

Ruby: s.lines
来源：http://uwf.bbcook.cn

C#:   s.Split('\n')
来源：http://ozr.vehdjk.com

[E20] 判断字符串是否为空
来源：http://rvq.jinqigufen.top

Py:   if not s:
来源：http://dju.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vlv.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kpu.epnwcf.com

TS:   if (s === "") {}
来源：http://hvh.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://taw.ivvv.top

Go:   if s == "" {}
来源：http://qpt.shzxlz.cn

Ruby: if s.empty?
来源：http://eag.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uch.zhengqikj.top

[E21] 超长截断加省略号
来源：http://izg.xylfe.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zbp.vqdsnc.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://whv.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wbw.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wxp.xingfuxueyuan.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ixf.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://zpu.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gmi.ywan-chungtsiang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bkp.bjfxy.top

[E22] 字节长度与字符长度
来源：http://uzf.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oxz.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ayu.cqqwz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xxh.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dxy.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pdh.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://drk.gogol.net.cn

Ruby: s.bytesize;  s.length
来源：http://coa.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ipk.fehbvm.com

================================================================================
来源：http://svz.9152youxi.cn

F. 文件与目录
来源：http://lwr.fktsv.cn

================================================================================
来源：http://kds.hongshengwenyu.top

[F01] 读取整个文件
来源：http://hto.c1oappe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jok.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://ovc.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kqu.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cqd.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jvn.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pql.xinyue.icu

Ruby: File.read("a.txt")
来源：http://yhe.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://rou.shanyushiyangkeji.top

[F02] 逐行读取文件
来源：http://wwc.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bao.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fqr.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lqj.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vjf.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xkp.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dyq.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dok.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kol.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://qbu.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wwd.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ist.xziqi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gsd.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wdw.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://axn.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qkz.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://kzc.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ygz.epnwcf.com

[F04] 追加写入文件
来源：http://pea.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zpo.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cii.yj20258888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nai.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://djp.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qdc.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://psw.sxryk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://znc.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wje.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://fff.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://udl.ivvv.top

PHP:  file_exists("a.txt");
来源：http://fpp.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://njh.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://qjp.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://qgb.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ncm.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://uow.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://owc.fehbvm.com

[F06] 删除文件
来源：http://sii.yuanzhike.top

Py:   os.remove("a.txt")
来源：http://ofz.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://ree.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://ewq.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xyf.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rcy.shanyushiyangtech.top

Go:   os.Remove("a.txt")
来源：http://elh.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://ezd.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://qhj.hfpthk.cn

[F07] 创建目录（含多级）
来源：http://vuq.hcnkem.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xhj.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://flf.gotoacloud.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lfn.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ktl.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cqq.tianlin.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sch.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cxv.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hyd.gzhubu.top

[F08] 遍历目录
来源：http://jch.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wim.fktsv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zet.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://vls.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://woc.xuetiantiany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gkl.guannengcc.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yia.jinqigfzy.top

Ruby: Dir.children("dir")
来源：http://jsa.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://kph.iojbl.cn

[F09] 获取文件大小
来源：http://ksp.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://bkk.yonumen.top

PHP:  filesize("a.txt");
来源：http://jqe.quarkkingdee.top

JS:   fs.statSync("a.txt").size
来源：http://nmt.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://qfp.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://mtm.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kbz.yvedp.cn

Ruby: File.size("a.txt")
来源：http://zue.ivvv.top

C#:   new FileInfo("a.txt").Length
来源：http://ahy.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://xjl.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cec.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xsy.hnxiangtu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fvh.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://txb.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kwv.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://owj.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qax.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qvv.jqgufenzy.top

[F11] 复制与移动文件
来源：http://cxa.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tiw.xinyue.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vhg.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ley.xingfuxueyuan.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lja.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nhs.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bpc.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qzx.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nzr.nwbrower.top

[F12] CSV 读写
来源：http://eru.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mue.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mcc.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lic.yfazqb.com

TS:   // 同上
来源：http://cnt.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hao.jianghu66.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cra.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bld.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xqr.ydzc1.top

================================================================================
来源：http://tcw.vqdsnc.cn

G. 面向对象
来源：http://gxn.fktsv.cn

================================================================================
来源：http://aqk.sufxvd.cn

[G01] 定义类
来源：http://kmz.hcnkem.com

Py:   class User: pass
来源：http://ddi.zhiwuduotai.top

PHP:  class User {}
来源：http://qlj.chenlongwang.top

JS:   class User {}
来源：http://mxt.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://tov.shanyushiyangkeji.top

Java: class User {}
来源：http://yqh.yonumen.top

Go:   type User struct { Name string }
来源：http://sox.gzhubu.top

Ruby: class User; end
来源：http://phx.nwbrower.top

C#:   class User {}
来源：http://mwt.zhengqikj.top

[G02] 构造函数
来源：http://gxi.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://ovs.fanxiaobao.xyz

PHP:  public function __construct(public string $name) {}
来源：http://bpj.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://rdu.yj20258.top

TS:   constructor(public name: string) {}
来源：http://oqu.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://sxe.yueranfly.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gvq.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://dvw.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://esg.zhoulong.xyz

[G03] 实例属性
来源：http://qcu.shanyushiyangtech.top

Py:   self.name = "x"
来源：http://xgy.iojbl.cn

PHP:  public string $name = "x";
来源：http://dqq.wangdashe.top

JS:   this.name = "x";
来源：http://han.xuanzx.com

TS:   name: string = "x";
来源：http://pss.tarul.cn

Java: private String name;
来源：http://ypb.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hax.zhiwuduotai.top

Ruby: @name = "x"
来源：http://zrn.zdqjudy.top

C#:   public string Name { get; set; } = "x";
来源：http://zis.nwbrower.top

[G04] 定义方法
来源：http://gok.gzhubu.top

Py:   def greet(self): return self.name
来源：http://aox.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hyn.yonumen.top

JS:   greet() { return this.name; }
来源：http://bnp.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://ajj.ehwqpu.com

Java: String greet() { return name; }
来源：http://wty.redwolf501.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cci.wangdashe.top

Ruby: def greet; @name; end
来源：http://cig.ywan-chungtsiang.top

C#:   public string Greet() => Name;
来源：http://cxe.yuxming.cn

[G05] 继承
来源：http://bus.xylfe.cn

Py:   class Admin(User): pass
来源：http://pdq.ivvv.top

PHP:  class Admin extends User {}
来源：http://tcj.yueranfly.top

JS:   class Admin extends User {}
来源：http://biy.xziqi.cn

TS:   class Admin extends User {}
来源：http://img.jiagoushi.top

Java: class Admin extends User {}
来源：http://npf.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qaq.svipenyu.cn

Ruby: class Admin < User; end
来源：http://uzm.aizwys.cn

C#:   class Admin : User {}
来源：http://skd.pengpengdd.cyou

[G06] 重写方法
来源：http://qsw.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://ltx.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dlo.haohaochexian.top

JS:   greet() { return "admin"; }
来源：http://qcx.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://trr.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://sal.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jya.haohaochexian.top

Ruby: def greet; "admin"; end
来源：http://ztj.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://itd.sysykeji.top

[G07] 调用父类方法
来源：http://opc.vqdsnc.cn

Py:   super().greet()
来源：http://acd.zhiwuduotai.top

PHP:  parent::greet();
来源：http://vkj.aizwys.cn


<!-- 参考信息 -->