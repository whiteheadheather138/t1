代发 wailian999

PHP:  implode(",", $items);
来源：http://rbw.zhixingplan.top

JS:   items.join(",")
来源：http://hxo.jyoumei.cn

TS:   items.join(",")
来源：http://apr.ydjk.org.cn

Java: String.join(",", items)
来源：http://oov.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://mjl.hnqzz.top

Ruby: items.join(",")
来源：http://imi.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://ieq.chenzaomai.com

[E09] 去除所有空白字符
来源：http://xam.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wcg.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fsi.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://znr.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://xkf.jiagoushi.top

Java: s.replaceAll("\\s+", "")
来源：http://ish.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tuy.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xks.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://acn.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://vsw.kuanghao11.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aqb.yfazqb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mmf.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://khf.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://axs.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://nta.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://atp.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sui.smart0.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bie.hnxiangtu.top

[E11] 反转字符串
来源：http://psm.yfazqb.com

Py:   s[::-1]
来源：http://nwu.sufxvd.cn

PHP:  strrev($s);
来源：http://drj.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://koo.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://sfu.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://aaa.cheryme.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jdt.hammf.cn

Ruby: s.reverse
来源：http://wdg.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://omt.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://wep.jyoumei.cn

Py:   s.count("a")
来源：http://gac.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://joo.pycfn.com

JS:   s.split("a").length - 1
来源：http://kdf.hongshengwenyu.top

TS:   s.split("a").length - 1
来源：http://kzx.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lmk.hammf.cn

Go:   strings.Count(s, "a")
来源：http://vuc.zdbjq.cn

Ruby: s.count("a")
来源：http://bdh.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://ogh.ydjk.org.cn

[E13] 逐字符遍历
来源：http://zgo.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://bja.zhaomingkeji.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://njh.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://hyk.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tuu.9152youxi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://owd.fengsongda.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wzc.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://arp.cqqwz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://are.fengsongda.top

[E14] URL 编码与 Base64
来源：http://vve.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mzi.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rra.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jbn.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kmc.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lct.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hcl.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lsi.shangyingyoupin.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tsi.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://vga.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mbq.jyoumei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rov.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://spl.bjfxy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://axn.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gcp.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tiw.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gue.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cgo.zhengqikj.top

[E16] 数字千分位
来源：http://rov.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://dtc.shuidangran.top

PHP:  number_format(1234567);
来源：http://ggy.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://geb.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://gtm.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dfb.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ank.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dfu.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://osy.zycfv.cn

[E17] 首字母大写
来源：http://hxk.sjlbkw.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://acp.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://peg.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qea.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dkh.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iir.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qlm.epnwcf.com

Ruby: s.capitalize
来源：http://dkz.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yce.tanke756.top

[E18] 模板占位符替换
来源：http://jac.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lfj.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jwc.sxryk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fxb.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kti.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qdn.chenlongwang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fos.zhixingplan.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kwp.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tev.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://mjh.sufxvd.cn

Py:   s.splitlines()
来源：http://uqo.shangyingyoupin.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pha.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://dkz.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://mwj.yangfankeji.com

Java: s.lines().toList()
来源：http://isc.yj20258.top

Go:   strings.Split(s, "\n")
来源：http://isk.yj20258888.top

Ruby: s.lines
来源：http://cfp.nanxuanxn.top

C#:   s.Split('\n')
来源：http://qql.tian-w.cn

[E20] 判断字符串是否为空
来源：http://fso.hnxiangtu.top

Py:   if not s:
来源：http://ztk.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zxi.jiagoushi.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kkr.52xcode.cn

TS:   if (s === "") {}
来源：http://yjp.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://lcx.hammf.cn

Go:   if s == "" {}
来源：http://owb.dashuyun.cn

Ruby: if s.empty?
来源：http://yse.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yci.shuidangran.top

[E21] 超长截断加省略号
来源：http://qff.yj20258888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://weu.ywan-chungtsiang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jwo.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wbg.guannengcc.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bqh.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blh.xziqi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ksl.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yhn.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bzm.smart0.xyz

[E22] 字节长度与字符长度
来源：http://mwe.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://prs.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vxz.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jrm.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tmc.yj20258888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eih.ivvv.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://htj.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://egz.xuetiantiany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kbe.hcnkem.com

================================================================================
来源：http://fel.gogol.net.cn

F. 文件与目录
来源：http://xzb.yj20258888.top

================================================================================
来源：http://nmq.zhijiandao.cn

[F01] 读取整个文件
来源：http://sgn.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iqy.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://sht.chenlongwang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hwk.0kj1m.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rdw.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zpd.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nfe.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://sli.jinyuanbaomall.cn

C#:   File.ReadAllText("a.txt");
来源：http://fss.316326.xyz

[F02] 逐行读取文件
来源：http://ipz.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lvm.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://brd.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jrh.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lps.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nrv.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aus.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rtr.hongshengwenyu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dif.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://ayy.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vfu.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://liy.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nvv.sufxvd.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rrr.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ilm.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fay.fanxiaobao.xyz

Ruby: File.write("a.txt", "hi")
来源：http://kbh.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://swl.ybcxt.top

[F04] 追加写入文件
来源：http://oek.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://whc.snrcjt.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qxi.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wyd.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gbf.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lml.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hlz.svipenyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yyh.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fgg.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://lkh.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iqg.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://zzf.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://dni.havefunace.top

TS:   fs.existsSync("a.txt")
来源：http://bhk.sysykeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yjz.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gap.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://fzj.tanke756.top

C#:   File.Exists("a.txt")
来源：http://nwu.vqdsnc.cn

[F06] 删除文件
来源：http://pwk.aizwys.cn

Py:   os.remove("a.txt")
来源：http://nbj.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://nmo.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://sun.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://hck.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://whz.yanxiufei.cn

Go:   os.Remove("a.txt")
来源：http://gvk.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://xup.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://cvp.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://ivk.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ojo.52xcode.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aoy.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://scd.wangdashe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yur.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kot.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://klb.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iss.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://txi.yj202588.top

[F08] 遍历目录
来源：http://tei.fengsongda.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tmi.shuidangran.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iur.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://fsp.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://alv.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ctj.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://eef.yj20258888.top

Ruby: Dir.children("dir")
来源：http://zwl.fzhhl.top

C#:   Directory.GetFiles("dir")
来源：http://gsl.yvedp.cn

[F09] 获取文件大小
来源：http://pka.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://omm.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://yzu.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://snb.yj20258888.top

TS:   fs.statSync("a.txt").size
来源：http://eeo.yuanzhike.top

Java: Files.size(Path.of("a.txt"))
来源：http://ogx.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gxo.xziqi.cn

Ruby: File.size("a.txt")
来源：http://wuv.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://kcn.tanke756.top

[F10] 取文件扩展名 / 文件名
来源：http://mkb.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://umk.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vjl.hesvh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://htv.iojbl.cn

TS:   path.extname("a.txt")
来源：http://acc.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://afw.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ilt.guowangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lay.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zmq.cqqwz.cn

[F11] 复制与移动文件
来源：http://gwc.jyoumei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nck.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mer.zhongyouzk.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tvf.xylfe.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yot.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xtn.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vog.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kng.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ihz.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://jua.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wtx.ybcxt.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wxw.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fcz.hcnkem.com

TS:   // 同上
来源：http://lag.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qha.yvedp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://byv.xuanzx.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bhn.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kag.jianghu66.top

================================================================================
来源：http://ntf.jyoumei.cn

G. 面向对象
来源：http://tgf.aizwys.cn

================================================================================
来源：http://fyl.zdqjudy.top

[G01] 定义类
来源：http://xsb.zdbjq.cn

Py:   class User: pass
来源：http://out.pycfn.com

PHP:  class User {}
来源：http://csq.wangdashe.top

JS:   class User {}
来源：http://iks.c1oappe.top

TS:   class User { name: string = ""; }
来源：http://qgp.jiagoushi.top

Java: class User {}
来源：http://yok.52xcode.cn

Go:   type User struct { Name string }
来源：http://cty.zhaomingkeji.xyz

Ruby: class User; end
来源：http://ofo.wangdashe.top

C#:   class User {}
来源：http://sjv.chenzaomai.com

[G02] 构造函数
来源：http://svw.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://mjs.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://ywh.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://vlr.tanke756.top

TS:   constructor(public name: string) {}
来源：http://tkk.jqgfzy.top

Java: User(String name) { this.name = name; }
来源：http://pll.bjfxy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wup.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://mmn.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://qax.fanxiaobao.xyz

[G03] 实例属性
来源：http://eyr.yj202588.top

Py:   self.name = "x"
来源：http://guz.hfpthk.cn

PHP:  public string $name = "x";
来源：http://pvj.nanxuanxn.top

JS:   this.name = "x";
来源：http://jaa.shzxlz.cn

TS:   name: string = "x";
来源：http://buc.snrcjt.cn

Java: private String name;
来源：http://gpf.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://buu.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://wnp.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://ftv.hcnkem.com

[G04] 定义方法
来源：http://yvv.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://bga.ppjwa.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bkv.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://wmk.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://hxt.daria6918.cn

Java: String greet() { return name; }
来源：http://mcn.xziqi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qpd.pengpengdd.cyou

Ruby: def greet; @name; end
来源：http://rqf.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://jtd.jyoumei.cn

[G05] 继承
来源：http://vpm.andypj.xyz

Py:   class Admin(User): pass
来源：http://rzl.chenlongwang.top

PHP:  class Admin extends User {}
来源：http://fgm.yonumen.top

JS:   class Admin extends User {}
来源：http://kzm.cashguo.top

TS:   class Admin extends User {}
来源：http://rmb.sxryk.cn

Java: class Admin extends User {}
来源：http://tuh.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qwa.dashuyun.cn

Ruby: class Admin < User; end
来源：http://npb.jinqigufen.top

C#:   class Admin : User {}
来源：http://tiy.fktsv.cn

[G06] 重写方法
来源：http://eae.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://ebl.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fmu.52xcode.cn

JS:   greet() { return "admin"; }
来源：http://rii.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://tdd.xingfuxueyuan.xyz

Java: @Override String greet() { return "admin"; }
来源：http://dep.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jik.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://mfg.gzhubu.top


<!-- 参考信息 -->