代发 wailian999

PHP:  implode(",", $items);
来源：http://ldv.fengsongda.top

JS:   items.join(",")
来源：http://ezr.jinyuanbaomall.cn

TS:   items.join(",")
来源：http://zrp.nwbrower.top

Java: String.join(",", items)
来源：http://sgy.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://ipg.uphjek.com

Ruby: items.join(",")
来源：http://aqt.shzxlz.cn

C#:   string.Join(",", items)
来源：http://wam.epnwcf.com

[E09] 去除所有空白字符
来源：http://gel.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://efr.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ynk.dianchejie.cn

JS:   s.replace(/\s+/g, "")
来源：http://xrs.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://uxt.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://ius.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ygh.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://ics.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wvb.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://ayk.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ryu.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://opy.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://aao.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://cxw.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://exs.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lwe.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mfa.jianghu66.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eix.uphjek.com

[E11] 反转字符串
来源：http://kzn.zhijiandao.cn

Py:   s[::-1]
来源：http://awh.sxryk.cn

PHP:  strrev($s);
来源：http://rre.yonumen.top

JS:   [...s].reverse().join("")
来源：http://vup.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://eze.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bzr.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jwh.9152youxi.cn

Ruby: s.reverse
来源：http://qft.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://xqa.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://qih.xingfuxueyuan.xyz

Py:   s.count("a")
来源：http://nxn.snrcjt.cn

PHP:  substr_count($s, "a");
来源：http://sio.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://mcd.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://yvd.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blt.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://okv.guannengcc.top

Ruby: s.count("a")
来源：http://jye.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://bfk.nanxuanxn.top

[E13] 逐字符遍历
来源：http://mno.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://xzl.hfpthk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://isb.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mtu.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://cet.mhx1999.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dzs.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://myh.gaohongyu789.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xub.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ptb.tian-w.cn

[E14] URL 编码与 Base64
来源：http://vif.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pjx.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lhe.shzxlz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tcv.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jle.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sml.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gnn.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vif.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zww.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://xuq.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hnm.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qjp.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://viv.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ipc.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lno.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jpv.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gof.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://irh.jiagoushi.top

[E16] 数字千分位
来源：http://cmn.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://erh.vehdjk.com

PHP:  number_format(1234567);
来源：http://tgy.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ihc.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lli.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aad.zhiwuduotai.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dbp.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rve.fanxiaobao.xyz

C#:   1234567.ToString("N0")
来源：http://xrk.vehdjk.com

[E17] 首字母大写
来源：http://tun.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hwb.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uyl.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://weq.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yzk.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qua.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rvn.fktsv.cn

Ruby: s.capitalize
来源：http://mdw.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bam.hfpthk.cn

[E18] 模板占位符替换
来源：http://auq.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jpq.ywan-chungtsiang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ynd.bbcook.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jph.xziqi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rvv.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aak.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tgb.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vpc.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vkz.fehbvm.com

[E19] 多行文本按行拆分
来源：http://nzl.hysaishi.cn

Py:   s.splitlines()
来源：http://zyu.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gmi.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://ire.hysaishi.cn

TS:   s.split(/\r?\n/)
来源：http://wez.yuanzhike.top

Java: s.lines().toList()
来源：http://pvs.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://bol.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://ccg.xinyue.icu

C#:   s.Split('\n')
来源：http://etm.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://nta.yongpay.top

Py:   if not s:
来源：http://wbj.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zaf.gogol.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://prj.jyoumei.cn

TS:   if (s === "") {}
来源：http://dsx.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://ckh.gotoacloud.top

Go:   if s == "" {}
来源：http://onx.52xcode.cn

Ruby: if s.empty?
来源：http://ksw.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://otw.52xcode.cn

[E21] 超长截断加省略号
来源：http://szy.yj20258888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nvq.zhiwuduotai.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qfu.jqgufenzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tda.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://agf.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ags.shanyushiyangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://wba.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hgo.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://djc.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://rrp.xuetiantiany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sci.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rxb.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dwj.0kj1m.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://npy.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oqy.gotoacloud.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://awh.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://uns.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xfm.yvedp.cn

================================================================================
来源：http://nic.c1oappe.top

F. 文件与目录
来源：http://chw.ywan-chungtsiang.top

================================================================================
来源：http://bkq.redwolf501.top

[F01] 读取整个文件
来源：http://ijg.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eaf.hywenlv.cn

PHP:  file_get_contents("a.txt");
来源：http://kgd.mhx1999.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://typ.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xun.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sin.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fpt.pycfn.com

Ruby: File.read("a.txt")
来源：http://jwh.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://qow.hfpthk.cn

[F02] 逐行读取文件
来源：http://xzc.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lwc.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pfk.daria6918.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nhq.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rhn.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vwk.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qhm.hammf.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://def.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mlv.daria6918.cn

[F03] 写入文件（覆盖）
来源：http://okg.jinghuilouyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fvn.yvedp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yac.shanyushiyangtech.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mdv.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dxn.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mpm.pengpengdd.cyou

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iyb.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://znq.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://efw.ctjpmb.com

[F04] 追加写入文件
来源：http://yyl.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tyg.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jfj.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xhg.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ahj.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mvr.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rcu.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mgf.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lpe.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://ojx.smart0.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rey.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://obz.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://wkl.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://kwj.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cvd.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://urf.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://jej.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://fwo.xuetiantiany.cn

[F06] 删除文件
来源：http://sca.xylfe.cn

Py:   os.remove("a.txt")
来源：http://obk.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://cjz.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://ckz.yj20258.top

TS:   fs.unlinkSync("a.txt")
来源：http://umu.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pbn.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://wyx.yj20258.top

Ruby: File.delete("a.txt")
来源：http://lpt.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://mie.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://wsb.jinqigfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hzx.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pgv.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yee.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://trn.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cbx.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sxq.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wuw.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hpa.sjlbkw.cn

[F08] 遍历目录
来源：http://oha.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ayy.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hkn.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://wzp.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://mdn.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tvh.sufxvd.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pwb.xziqi.cn

Ruby: Dir.children("dir")
来源：http://uaq.havefunace.top

C#:   Directory.GetFiles("dir")
来源：http://ylg.shuidangran.top

[F09] 获取文件大小
来源：http://bbk.yueranfly.top

Py:   os.path.getsize("a.txt")
来源：http://vgs.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://zhu.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://vvt.redwolf501.top

TS:   fs.statSync("a.txt").size
来源：http://isb.hnxiangtu.top

Java: Files.size(Path.of("a.txt"))
来源：http://wwd.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wqe.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://lqa.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://iho.ywan-chungtsiang.top

[F10] 取文件扩展名 / 文件名
来源：http://cwc.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ezv.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qgg.dashuyun.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ynq.shuidangran.top

TS:   path.extname("a.txt")
来源：http://blt.vqdsnc.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://odb.hcnkem.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xqd.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qxf.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hee.tanke756.top

[F11] 复制与移动文件
来源：http://gxw.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bdm.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://owh.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fyd.xuetiantiany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ihd.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ftf.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cbz.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ecn.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yyl.yuanzhike.top

[F12] CSV 读写
来源：http://uks.cucudq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gce.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cbc.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mhw.jqgfzy.top

TS:   // 同上
来源：http://zqf.feifeiyinyue.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wcd.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://igg.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nwx.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gjz.zhaomingkeji.xyz

================================================================================
来源：http://kbr.zhoulong.xyz

G. 面向对象
来源：http://zik.yuxming.cn

================================================================================
来源：http://qtk.zhixingplan.top

[G01] 定义类
来源：http://ucb.jyoumei.cn

Py:   class User: pass
来源：http://bib.jinyuanbaomall.cn

PHP:  class User {}
来源：http://agu.redwolf501.top

JS:   class User {}
来源：http://jlz.yanxiufei.cn

TS:   class User { name: string = ""; }
来源：http://zvl.quarkkingdee.top

Java: class User {}
来源：http://yah.tianlin.xyz

Go:   type User struct { Name string }
来源：http://nra.fanxiaobao.xyz

Ruby: class User; end
来源：http://tbk.zhongyouzk.top

C#:   class User {}
来源：http://ugc.fehbvm.com

[G02] 构造函数
来源：http://vyh.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://mzr.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://wdl.316326.xyz

JS:   constructor(name) { this.name = name; }
来源：http://fsf.vehdjk.com

TS:   constructor(public name: string) {}
来源：http://sht.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://jbq.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hkb.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://fpm.ppjwa.cn

C#:   public User(string name) { Name = name; }
来源：http://ayx.jiagoushi.top

[G03] 实例属性
来源：http://irj.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://lnd.hammf.cn

PHP:  public string $name = "x";
来源：http://sev.xingfuxueyuan.xyz

JS:   this.name = "x";
来源：http://ygd.hongshengwenyu.top

TS:   name: string = "x";
来源：http://ork.aizwys.cn

Java: private String name;
来源：http://hpa.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mla.sweek.top

Ruby: @name = "x"
来源：http://hth.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://cwu.sysykeji.top

[G04] 定义方法
来源：http://zty.mhx1999.top

Py:   def greet(self): return self.name
来源：http://grv.shanyushiyangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://eyn.yueranfly.top

JS:   greet() { return this.name; }
来源：http://uun.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://pms.cqqwz.cn

Java: String greet() { return name; }
来源：http://wmn.tarul.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mcx.yvedp.cn

Ruby: def greet; @name; end
来源：http://qab.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://day.xylfe.cn

[G05] 继承
来源：http://inn.316326.xyz

Py:   class Admin(User): pass
来源：http://stz.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://kdh.yonumen.top

JS:   class Admin extends User {}
来源：http://gzj.jinqigfzy.top

TS:   class Admin extends User {}
来源：http://llt.yuanzhike.top

Java: class Admin extends User {}
来源：http://cgh.nwbrower.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wzo.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://skf.fehbvm.com

C#:   class Admin : User {}
来源：http://dds.cucudq.cn

[G06] 重写方法
来源：http://jip.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://lke.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://uqz.nwbrower.top

JS:   greet() { return "admin"; }
来源：http://cgt.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://csm.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://nwr.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zil.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://ado.nwbrower.top


<!-- 参考信息 -->