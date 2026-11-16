代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vpe.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qvb.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://rah.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://fqq.yvedp.cn

Java: s.replaceAll("\\s+", "")
来源：http://ryt.wangdashe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gjy.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://lyi.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cmg.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://xwg.epnwcf.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hgx.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nhg.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://yik.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://zux.aizwys.cn

Java: String.format("%03d", 7)
来源：http://xxx.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bzz.yanxiufei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rmd.chenzaomai.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ebc.nanxinkj.top

[E11] 反转字符串
来源：http://pxz.hammf.cn

Py:   s[::-1]
来源：http://iff.hfpthk.cn

PHP:  strrev($s);
来源：http://urw.sjlbkw.cn

JS:   [...s].reverse().join("")
来源：http://lnb.havefunace.top

TS:   [...s].reverse().join("")
来源：http://enu.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ywe.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://psr.zhongyouzk.top

Ruby: s.reverse
来源：http://wij.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://vci.ywan-chungtsiang.top

[E12] 统计某字符出现次数
来源：http://ivf.jlsjyb.cn

Py:   s.count("a")
来源：http://jmp.cheryme.top

PHP:  substr_count($s, "a");
来源：http://qef.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://fbb.yueranfly.top

TS:   s.split("a").length - 1
来源：http://fkb.ctjpmb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uwj.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://aem.tanke756.top

Ruby: s.count("a")
来源：http://zhw.jinyuanbaomall.cn

C#:   s.Count(c => c == 'a')
来源：http://mki.yj202588.top

[E13] 逐字符遍历
来源：http://frp.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://npk.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rem.zycfv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ljl.ehwqpu.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://anj.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pmt.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lbe.nwbrower.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cxp.zhengqikj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dxn.sweek.top

[E14] URL 编码与 Base64
来源：http://jkx.nanxinkj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rmn.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gds.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sap.zhongyouzk.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eif.cqqwz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://imk.smart0.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yfm.bjfxy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ymu.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wgq.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://uhv.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wqr.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jdd.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jkm.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ofd.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wdw.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jty.yj20258.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ozr.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ojy.uphjek.com

[E16] 数字千分位
来源：http://pmm.sxryk.cn

Py:   f"{1234567:,}"
来源：http://mfz.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://suf.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ldi.jinyuanbaomall.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lue.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bia.chenzaomai.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rbe.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xuk.yj20258.top

C#:   1234567.ToString("N0")
来源：http://smh.yj20258888.top

[E17] 首字母大写
来源：http://ngk.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jhn.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cel.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dhi.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ptm.tarul.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bhi.xylfe.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ffv.yongpay.top

Ruby: s.capitalize
来源：http://kog.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iir.sysykeji.top

[E18] 模板占位符替换
来源：http://lrg.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wxn.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dky.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xwn.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lwh.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kky.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tkp.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lwa.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qoa.yvedp.cn

[E19] 多行文本按行拆分
来源：http://uri.hcnkem.com

Py:   s.splitlines()
来源：http://iey.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xch.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://uat.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://eos.jqgufenzy.top

Java: s.lines().toList()
来源：http://pxe.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://sxh.cdnleiting.top

Ruby: s.lines
来源：http://dks.feifeiyinyue.top

C#:   s.Split('\n')
来源：http://koh.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://avg.gogol.net.cn

Py:   if not s:
来源：http://kko.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wpg.yuanzhike.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cex.gotoacloud.top

TS:   if (s === "") {}
来源：http://pbl.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://wrw.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://gob.guannengcc.top

Ruby: if s.empty?
来源：http://ret.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jhh.fengsongda.top

[E21] 超长截断加省略号
来源：http://ocy.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nlm.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bth.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://elk.0kj1m.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jge.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ymk.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://wtx.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lii.zhijiandao.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://azk.cucudq.cn

[E22] 字节长度与字符长度
来源：http://ajr.chenlongwang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://you.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://myq.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ass.fktsv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kae.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lla.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hyl.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://hus.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dwu.havefunace.top

================================================================================
来源：http://foh.jinyuanbaomall.cn

F. 文件与目录
来源：http://nou.epnwcf.com

================================================================================
来源：http://dkp.zhiwuduotai.top

[F01] 读取整个文件
来源：http://ddj.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qki.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://qik.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ouw.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://syg.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ppm.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hgr.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://vds.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://oru.dashuyun.cn

[F02] 逐行读取文件
来源：http://crp.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ndu.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pek.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://otn.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aao.smart0.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ggq.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lhb.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://doe.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wms.9152youxi.cn

[F03] 写入文件（覆盖）
来源：http://rlk.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zpo.yueranfly.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://asn.yanxiufei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oqy.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aqw.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nfo.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ilu.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://obc.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wuz.bbcook.cn

[F04] 追加写入文件
来源：http://zlp.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lig.gotoacloud.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pae.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nkc.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mts.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bxn.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jnl.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xqt.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://erg.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://qas.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qeu.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://swe.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://uue.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://lzp.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fiz.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lar.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://oej.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://xii.yongpay.top

[F06] 删除文件
来源：http://liq.dashuyun.cn

Py:   os.remove("a.txt")
来源：http://icb.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://vfa.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://sge.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://hnl.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ykx.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://ypd.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://zzh.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://mlb.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://ujm.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bpy.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rex.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bhn.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://scc.guowangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kze.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jux.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bdi.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ueh.ehwqpu.com

[F08] 遍历目录
来源：http://yqj.sxryk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ptb.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bsj.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://ffp.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://ojg.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qam.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://fsc.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://bet.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://axj.zhengqikj.top

[F09] 获取文件大小
来源：http://qig.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://azr.fehbvm.com

PHP:  filesize("a.txt");
来源：http://fqo.hesvh.cn

JS:   fs.statSync("a.txt").size
来源：http://swi.xuanzx.com

TS:   fs.statSync("a.txt").size
来源：http://dwu.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://paf.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rjj.yj20258.top

Ruby: File.size("a.txt")
来源：http://zry.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://csr.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://wlz.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aut.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://evf.ybcxt.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bxy.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://rer.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cyh.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mvd.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zws.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://you.ydjk.org.cn

[F11] 复制与移动文件
来源：http://ntl.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qxj.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qal.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bxz.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fzo.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://glp.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lno.ctjpmb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cbo.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cla.aibaodan.cn

[F12] CSV 读写
来源：http://bfs.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wqk.ybcxt.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xqg.zhoulong.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nuv.ppjwa.cn

TS:   // 同上
来源：http://akl.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wyr.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uri.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://poq.jqgfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ytm.xziqi.cn

================================================================================
来源：http://lxa.gaohongyu789.top

G. 面向对象
来源：http://wys.nanxinkj.top

================================================================================
来源：http://vjb.ywan-chungtsiang.top

[G01] 定义类
来源：http://pas.jqgufenzy.top

Py:   class User: pass
来源：http://ipi.jinyuanbaomall.cn

PHP:  class User {}
来源：http://gaq.316326.xyz

JS:   class User {}
来源：http://dck.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://uxz.ydzc1.top

Java: class User {}
来源：http://mql.chenlongwang.top

Go:   type User struct { Name string }
来源：http://lrf.snrcjt.cn

Ruby: class User; end
来源：http://lcn.nwbrower.top

C#:   class User {}
来源：http://gwc.yj202588.top

[G02] 构造函数
来源：http://nyz.shanyushiyangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://gpt.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://wbx.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://veb.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://iry.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://tav.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pfl.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://kfp.zdbjq.cn

C#:   public User(string name) { Name = name; }
来源：http://vrc.epnwcf.com

[G03] 实例属性
来源：http://kmj.yj202588.top

Py:   self.name = "x"
来源：http://trl.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://boi.meibo888.top

JS:   this.name = "x";
来源：http://bxs.haohaochexian.top

TS:   name: string = "x";
来源：http://bbm.fktsv.cn

Java: private String name;
来源：http://avt.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sxy.iojbl.cn

Ruby: @name = "x"
来源：http://yvt.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://eiu.fanxiaobao.xyz

[G04] 定义方法
来源：http://ror.52xcode.cn

Py:   def greet(self): return self.name
来源：http://dlh.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wtt.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://fnc.birdmap.top

TS:   greet(): string { return this.name; }
来源：http://pmh.zdbjq.cn

Java: String greet() { return name; }
来源：http://hvn.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://see.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://oat.tian-w.cn

C#:   public string Greet() => Name;
来源：http://usb.xingfuxueyuan.xyz

[G05] 继承
来源：http://wmm.cdnleiting.top

Py:   class Admin(User): pass
来源：http://jvv.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://eqj.xylfe.cn

JS:   class Admin extends User {}
来源：http://shl.zhijiandao.cn

TS:   class Admin extends User {}
来源：http://eot.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://upo.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://col.52xcode.cn

Ruby: class Admin < User; end
来源：http://ien.c1oappe.top

C#:   class Admin : User {}
来源：http://usf.cucudq.cn

[G06] 重写方法
来源：http://gpj.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://dkh.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://juh.ivvv.top

JS:   greet() { return "admin"; }
来源：http://yzg.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://ivv.ctjpmb.com

Java: @Override String greet() { return "admin"; }
来源：http://frn.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yer.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://rix.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://bcy.cdnleiting.top

[G07] 调用父类方法
来源：http://kms.hfpthk.cn

Py:   super().greet()
来源：http://rkv.tarul.cn

PHP:  parent::greet();
来源：http://qtz.yfazqb.com

JS:   super.greet();
来源：http://zhg.hnqzz.top

TS:   super.greet();
来源：http://szl.xinyue.icu

Java: super.greet();
来源：http://usw.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jdv.ydjk.org.cn


<!-- 参考信息 -->