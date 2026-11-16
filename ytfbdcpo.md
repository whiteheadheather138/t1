代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://vuz.cucudq.cn

TS:   s.split(",")
来源：http://rio.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ido.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wsh.quarkkingdee.top

Ruby: s.split(",");  s.split
来源：http://vry.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dks.nwbrower.top

[E08] 数组按分隔符合并
来源：http://mmg.meibo888.top

Py:   ",".join(items)
来源：http://wzz.epnwcf.com

PHP:  implode(",", $items);
来源：http://txq.zhoulong.xyz

JS:   items.join(",")
来源：http://xjf.yj20258.top

TS:   items.join(",")
来源：http://uai.ehwqpu.com

Java: String.join(",", items)
来源：http://krk.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://yfs.yvedp.cn

Ruby: items.join(",")
来源：http://rcn.zhixingplan.top

C#:   string.Join(",", items)
来源：http://wnj.sweek.top

[E09] 去除所有空白字符
来源：http://wpj.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://enh.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rmm.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://ppe.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://eol.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://eah.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mto.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://uej.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eux.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://hwa.guannengcc.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ywt.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yek.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://sbw.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://dzv.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://ycd.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nto.fzhhl.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://szb.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ogd.pycfn.com

[E11] 反转字符串
来源：http://qic.xinyue.icu

Py:   s[::-1]
来源：http://ncr.feifeiyinyue.top

PHP:  strrev($s);
来源：http://ogv.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://qae.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://qso.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iqn.meibo888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mvi.hnqzz.top

Ruby: s.reverse
来源：http://aff.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dba.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://mio.xingfuxueyuan.xyz

Py:   s.count("a")
来源：http://jsl.zhongyouzk.top

PHP:  substr_count($s, "a");
来源：http://wos.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://dlm.shangyingyoupin.top

TS:   s.split("a").length - 1
来源：http://onn.daria6918.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://voq.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://sdq.yanxiufei.cn

Ruby: s.count("a")
来源：http://ild.ywan-chungtsiang.top

C#:   s.Count(c => c == 'a')
来源：http://yte.sweek.top

[E13] 逐字符遍历
来源：http://amf.ybcxt.top

Py:   for ch in s: print(ch)
来源：http://pdq.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tug.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://hsf.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://moh.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mtv.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xxd.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://loa.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tqq.0kj1m.cn

[E14] URL 编码与 Base64
来源：http://ppc.redwolf501.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vya.ehwqpu.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://kex.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blb.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://and.cashguo.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ypb.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zfd.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kdi.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qyo.ybcxt.top

[E15] HTML 转义 / 反转义
来源：http://wsp.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://isw.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xji.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://njl.jianghu66.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bai.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fkv.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iob.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bfk.snrcjt.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ejr.vqdsnc.cn

[E16] 数字千分位
来源：http://qiw.nwbrower.top

Py:   f"{1234567:,}"
来源：http://qts.chenlongwang.top

PHP:  number_format(1234567);
来源：http://edv.snrcjt.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nqq.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://zmw.zhongyouzk.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wsr.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yup.chenzaomai.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://azl.uphjek.com

C#:   1234567.ToString("N0")
来源：http://qdp.cqqwz.cn

[E17] 首字母大写
来源：http://fct.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ucj.sufxvd.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yrj.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nke.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://thy.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://keb.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://udg.ppjwa.cn

Ruby: s.capitalize
来源：http://pos.zycfv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gcr.aizwys.cn

[E18] 模板占位符替换
来源：http://qqf.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tgn.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mxh.guannengcc.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qmy.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wsu.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lmy.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bma.xylfe.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://czn.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rnw.smart0.xyz

[E19] 多行文本按行拆分
来源：http://dgu.nwbrower.top

Py:   s.splitlines()
来源：http://trm.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ooo.chenzaomai.com

JS:   s.split(/\r?\n/)
来源：http://pbn.shzxlz.cn

TS:   s.split(/\r?\n/)
来源：http://xyd.chenzaomai.com

Java: s.lines().toList()
来源：http://vee.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://hws.yueranfly.top

Ruby: s.lines
来源：http://ocs.daria6918.cn

C#:   s.Split('\n')
来源：http://wha.fehbvm.com

[E20] 判断字符串是否为空
来源：http://ube.hnqzz.top

Py:   if not s:
来源：http://wdl.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uzk.zycfv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wxc.cheryme.top

TS:   if (s === "") {}
来源：http://aja.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://xld.xylfe.cn

Go:   if s == "" {}
来源：http://gdp.tianlin.xyz

Ruby: if s.empty?
来源：http://jkf.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://exz.shzxlz.cn

[E21] 超长截断加省略号
来源：http://pfo.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xpw.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://azo.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mvl.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rwt.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://glm.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://wdw.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://utx.0kj1m.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://phm.shanyushiyangkeji.top

[E22] 字节长度与字符长度
来源：http://igq.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jge.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zou.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vjl.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wuo.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pxz.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zsh.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://cgi.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://klr.jiagoushi.top

================================================================================
来源：http://lmm.cqqwz.cn

F. 文件与目录
来源：http://mea.mhx1999.top

================================================================================
来源：http://baj.xuetiantiany.cn

[F01] 读取整个文件
来源：http://ogg.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zqa.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://zuu.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://umy.jianghu66.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bhe.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xhh.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://flm.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://qtd.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://uof.epnwcf.com

[F02] 逐行读取文件
来源：http://jxn.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wtx.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ycw.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://omk.sysykeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yvf.gotoacloud.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pnv.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gox.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bhg.guowangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jdy.quarkkingdee.top

[F03] 写入文件（覆盖）
来源：http://rwh.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ltd.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qzq.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://thx.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xui.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kwo.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gig.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://htf.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zev.yonumen.top

[F04] 追加写入文件
来源：http://ahg.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rpj.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yrr.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uli.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zpu.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lwc.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oyt.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aya.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bhd.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://ayh.zhoulong.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iib.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://fsm.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://xpk.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://sye.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://msj.wangshuangyany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mds.sweek.top

Ruby: File.exist?("a.txt")
来源：http://pcm.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://uay.yongpay.top

[F06] 删除文件
来源：http://rgz.cqqwz.cn

Py:   os.remove("a.txt")
来源：http://qeb.bjfxy.top

PHP:  unlink("a.txt");
来源：http://slv.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://ffv.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qlc.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uzv.zhixingplan.top

Go:   os.Remove("a.txt")
来源：http://fja.shanyushiyangkeji.top

Ruby: File.delete("a.txt")
来源：http://nwg.yj20258.top

C#:   File.Delete("a.txt");
来源：http://mbl.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://myg.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pjw.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lur.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nco.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aim.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wma.ppjwa.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iwc.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cwp.jinqigfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://exe.guowangkeji.top

[F08] 遍历目录
来源：http://ici.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cns.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rql.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://lej.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://fyk.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ygp.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hyj.guannengcc.top

Ruby: Dir.children("dir")
来源：http://unl.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://jsz.kuanghao11.cn

[F09] 获取文件大小
来源：http://ohl.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://kky.chenlongwang.top

PHP:  filesize("a.txt");
来源：http://qlp.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://aap.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://zzz.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zhf.xingfuxueyuan.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fel.pycfn.com

Ruby: File.size("a.txt")
来源：http://jct.zhaomingkeji.xyz

C#:   new FileInfo("a.txt").Length
来源：http://hdu.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://qww.cqqwz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hdl.hongshengwenyu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wnd.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ivt.yonumen.top

TS:   path.extname("a.txt")
来源：http://rxk.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kui.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://byj.cashguo.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ehc.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kyn.smart0.xyz

[F11] 复制与移动文件
来源：http://xap.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://irj.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xuj.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mry.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aix.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gsm.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rje.hnxiangtu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aof.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://koe.shuidangran.top

[F12] CSV 读写
来源：http://wrk.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dti.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://apu.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dir.cucudq.cn

TS:   // 同上
来源：http://pke.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qnl.fengsongda.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rhk.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nvc.0kj1m.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jrj.cqqwz.cn

================================================================================
来源：http://ezw.fehbvm.com

G. 面向对象
来源：http://yhd.guannengcc.top

================================================================================
来源：http://jvd.c1oappe.top

[G01] 定义类
来源：http://rap.hammf.cn

Py:   class User: pass
来源：http://snj.zdqjudy.top

PHP:  class User {}
来源：http://las.pengpengdd.cyou

JS:   class User {}
来源：http://fmb.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://eih.vqdsnc.cn

Java: class User {}
来源：http://tag.guowangkeji.top

Go:   type User struct { Name string }
来源：http://tmq.zhoulong.xyz

Ruby: class User; end
来源：http://olk.ybcxt.top

C#:   class User {}
来源：http://oml.zhongyouzk.top

[G02] 构造函数
来源：http://isi.wangshuangyany.cn

Py:   def __init__(self, name): self.name = name
来源：http://xee.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://obe.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://emk.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://ckl.c1oappe.top

Java: User(String name) { this.name = name; }
来源：http://arp.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://anj.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://dld.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://eqz.sufxvd.cn

[G03] 实例属性
来源：http://reo.dashuyun.cn

Py:   self.name = "x"
来源：http://xuc.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://kig.xylfe.cn

JS:   this.name = "x";
来源：http://mou.xziqi.cn

TS:   name: string = "x";
来源：http://gju.nanxuanxn.top

Java: private String name;
来源：http://esc.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mcu.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://vdf.chenzaomai.com

C#:   public string Name { get; set; } = "x";
来源：http://ovn.fanxiaobao.xyz

[G04] 定义方法
来源：http://wzw.yfazqb.com

Py:   def greet(self): return self.name
来源：http://vwe.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pat.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://wjp.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://hqe.cdnleiting.top

Java: String greet() { return name; }
来源：http://gro.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://uea.yvedp.cn

Ruby: def greet; @name; end
来源：http://ybl.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://yek.ybcxt.top

[G05] 继承
来源：http://rgd.zhixingplan.top

Py:   class Admin(User): pass
来源：http://enz.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://qhd.fehbvm.com

JS:   class Admin extends User {}
来源：http://hhr.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://rsn.cdnleiting.top

Java: class Admin extends User {}
来源：http://bzl.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ktp.ydjk.org.cn

Ruby: class Admin < User; end
来源：http://rbd.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://vww.chenzaomai.com


<!-- 参考信息 -->