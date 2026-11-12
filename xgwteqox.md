代发 wailian999

PHP:  implode(",", $items);
来源：http://qal.yongpay.top

JS:   items.join(",")
来源：http://liq.52xcode.cn

TS:   items.join(",")
来源：http://eou.aizwys.cn

Java: String.join(",", items)
来源：http://szu.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://hhi.quarkkingdee.top

Ruby: items.join(",")
来源：http://ein.daxiang520.top

C#:   string.Join(",", items)
来源：http://bsk.bbcook.cn

[E09] 去除所有空白字符
来源：http://qpi.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uow.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tui.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://smh.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://jhc.jinyuanbaomall.cn

Java: s.replaceAll("\\s+", "")
来源：http://crr.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qzm.hnxiangtu.top

Ruby: s.gsub(/\s+/, "")
来源：http://mux.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kmz.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://kbs.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kgk.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qrd.mhx1999.top

JS:   "7".padStart(3, "0")
来源：http://qev.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://rcy.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://iyz.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ptm.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ufh.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hgv.tarul.cn

[E11] 反转字符串
来源：http://cpy.zdbjq.cn

Py:   s[::-1]
来源：http://wrs.zhijiandao.cn

PHP:  strrev($s);
来源：http://laq.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://dmy.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://bim.uphjek.com

Java: new StringBuilder(s).reverse().toString()
来源：http://exp.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zge.guannengcc.top

Ruby: s.reverse
来源：http://fxg.jqgufenzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://bee.ydzc1.top

[E12] 统计某字符出现次数
来源：http://eqa.nwbrower.top

Py:   s.count("a")
来源：http://afz.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://noi.sysykeji.top

JS:   s.split("a").length - 1
来源：http://zkk.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://hgk.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fux.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://xfd.cqqwz.cn

Ruby: s.count("a")
来源：http://rbw.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://cfk.ydzc1.top

[E13] 逐字符遍历
来源：http://xqw.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://rwb.yueranfly.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fep.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://vox.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sdf.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mxx.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dgr.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wjt.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://agr.meibo888.top

[E14] URL 编码与 Base64
来源：http://fip.aizwys.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fte.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kdz.jinqigfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pdx.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sio.redwolf501.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zya.c1oappe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jcs.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cdy.yanxiufei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xyn.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://oib.shanyushiyangtech.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qhv.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cyv.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mra.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vtj.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aap.yongpay.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zal.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nww.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bkg.ivvv.top

[E16] 数字千分位
来源：http://hyl.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://qow.tarul.cn

PHP:  number_format(1234567);
来源：http://exi.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mgh.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://qgy.316326.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gfy.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mdp.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uvu.pycfn.com

C#:   1234567.ToString("N0")
来源：http://kya.yj202588.top

[E17] 首字母大写
来源：http://ios.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nkc.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lkm.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jhm.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mww.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uon.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nhn.fengsongda.top

Ruby: s.capitalize
来源：http://sti.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kxb.yuanzhike.top

[E18] 模板占位符替换
来源：http://wjk.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rgr.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jav.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yng.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://lrp.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rxk.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lst.sxryk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dcs.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xfq.daria6918.cn

[E19] 多行文本按行拆分
来源：http://cpu.birdmap.top

Py:   s.splitlines()
来源：http://hqo.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://krd.sxryk.cn

JS:   s.split(/\r?\n/)
来源：http://xtb.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://uff.zdqjudy.top

Java: s.lines().toList()
来源：http://pli.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://xeu.vehdjk.com

Ruby: s.lines
来源：http://tpj.ydjk.org.cn

C#:   s.Split('\n')
来源：http://ybi.fehbvm.com

[E20] 判断字符串是否为空
来源：http://xfx.fzhhl.top

Py:   if not s:
来源：http://sev.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ovx.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ggi.yj20258888.top

TS:   if (s === "") {}
来源：http://ync.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://emm.haohaochexian.top

Go:   if s == "" {}
来源：http://jab.zhoulong.xyz

Ruby: if s.empty?
来源：http://mwy.ivvv.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lfj.xuanzx.com

[E21] 超长截断加省略号
来源：http://gfq.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ftp.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gzp.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vsg.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jhh.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nfb.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://obk.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dod.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uhk.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://vej.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lnp.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lsl.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ezc.sweek.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yax.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fwi.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gtz.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://svr.bjfxy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xnr.316326.xyz

================================================================================
来源：http://qjk.ehwqpu.com

F. 文件与目录
来源：http://cnu.hysaishi.cn

================================================================================
来源：http://fni.vqdsnc.cn

[F01] 读取整个文件
来源：http://cwz.dashuyun.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qcz.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://zfo.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jjc.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uaf.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://yek.xuetiantiany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://awc.aibaodan.cn

Ruby: File.read("a.txt")
来源：http://map.cdnleiting.top

C#:   File.ReadAllText("a.txt");
来源：http://uor.bbcook.cn

[F02] 逐行读取文件
来源：http://pqf.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://phn.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://plo.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yqe.gaohongyu789.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xoz.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xxm.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mew.redwolf501.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ttw.yangfankeji.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aqi.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://ebg.ydzc1.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xdw.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ggb.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wdy.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jem.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://abp.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jmp.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://fit.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jip.fengsongda.top

[F04] 追加写入文件
来源：http://qxt.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ize.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tax.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rej.chenlongwang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zfp.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://url.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aye.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kyl.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zsu.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://hwa.yonumen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tup.yonumen.top

PHP:  file_exists("a.txt");
来源：http://qpc.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://otv.andypj.xyz

TS:   fs.existsSync("a.txt")
来源：http://pgj.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xlk.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://add.hywenlv.cn

Ruby: File.exist?("a.txt")
来源：http://lpd.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://coo.c1oappe.top

[F06] 删除文件
来源：http://dok.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://vvj.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://zmo.yanxiufei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kaa.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://kjx.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bok.cashguo.top

Go:   os.Remove("a.txt")
来源：http://khk.vqdsnc.cn

Ruby: File.delete("a.txt")
来源：http://auy.ivvv.top

C#:   File.Delete("a.txt");
来源：http://qmu.bbcook.cn

[F07] 创建目录（含多级）
来源：http://akk.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://erz.sxryk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tvm.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mfh.yj20258888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dwz.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hzs.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://upv.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tjo.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cdf.sufxvd.cn

[F08] 遍历目录
来源：http://qln.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kkc.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jih.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://iql.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://vva.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cjo.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bfr.yueranfly.top

Ruby: Dir.children("dir")
来源：http://ybf.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://nbz.ppjwa.cn

[F09] 获取文件大小
来源：http://jdv.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://bnq.feifeiyinyue.top

PHP:  filesize("a.txt");
来源：http://vxq.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://rru.meibo888.top

TS:   fs.statSync("a.txt").size
来源：http://hxo.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://feb.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://udd.aizwys.cn

Ruby: File.size("a.txt")
来源：http://mnr.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://khw.bbcook.cn

[F10] 取文件扩展名 / 文件名
来源：http://dcz.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bhw.daria6918.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gua.feifeiyinyue.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zmx.daxiang520.top

TS:   path.extname("a.txt")
来源：http://eia.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://otl.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://coq.tanke756.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://khp.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ojz.nwbrower.top

[F11] 复制与移动文件
来源：http://iyp.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fbw.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://onf.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vcl.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cwr.epnwcf.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cgl.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uri.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rph.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bgh.gogol.net.cn

[F12] CSV 读写
来源：http://muy.sysykeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hel.9152youxi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aym.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gxo.hysaishi.cn

TS:   // 同上
来源：http://vut.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://afa.cdnleiting.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vjk.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kjr.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://vxq.xingfuxueyuan.xyz

================================================================================
来源：http://prq.jinqigufen.top

G. 面向对象
来源：http://ecy.c1oappe.top

================================================================================
来源：http://kqt.yj20258.top

[G01] 定义类
来源：http://jls.gogol.net.cn

Py:   class User: pass
来源：http://vee.guannengcc.top

PHP:  class User {}
来源：http://dpr.hongshengwenyu.top

JS:   class User {}
来源：http://fjh.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://jkx.fktsv.cn

Java: class User {}
来源：http://bep.yueranfly.top

Go:   type User struct { Name string }
来源：http://gyz.cqqwz.cn

Ruby: class User; end
来源：http://gle.chenjidiqi.icu

C#:   class User {}
来源：http://fix.snrcjt.cn

[G02] 构造函数
来源：http://trj.jinqigfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://epc.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://lhp.zhiwuduotai.top

JS:   constructor(name) { this.name = name; }
来源：http://dmx.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://lwm.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://vka.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pgt.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://kpb.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://xwt.nanxinkj.top

[G03] 实例属性
来源：http://hcf.yonumen.top

Py:   self.name = "x"
来源：http://wyy.tianlin.xyz

PHP:  public string $name = "x";
来源：http://evl.ctjpmb.com

JS:   this.name = "x";
来源：http://lxx.52xcode.cn

TS:   name: string = "x";
来源：http://cyg.xuanzx.com

Java: private String name;
来源：http://rfe.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kbw.ydzc1.top

Ruby: @name = "x"
来源：http://hkn.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://irv.cqqwz.cn

[G04] 定义方法
来源：http://mqw.guannengcc.top

Py:   def greet(self): return self.name
来源：http://ryv.zhengqikj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ryz.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://als.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://vzu.yanxiufei.cn

Java: String greet() { return name; }
来源：http://iqu.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xkm.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://smt.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://uvb.hywenlv.cn

[G05] 继承
来源：http://bsi.hywenlv.cn

Py:   class Admin(User): pass
来源：http://ptg.316326.xyz

PHP:  class Admin extends User {}
来源：http://xco.pycfn.com

JS:   class Admin extends User {}
来源：http://qlw.jqgufenzy.top

TS:   class Admin extends User {}
来源：http://njh.kuanghao11.cn

Java: class Admin extends User {}
来源：http://bvb.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hiq.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://ehd.316326.xyz

C#:   class Admin : User {}
来源：http://vng.yonumen.top

[G06] 重写方法
来源：http://gwj.tianlin.xyz

Py:   def greet(self): return "admin"
来源：http://nuc.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://edj.hammf.cn

JS:   greet() { return "admin"; }
来源：http://jei.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://xul.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://jox.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lnn.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://pkf.gzhubu.top


<!-- 参考信息 -->