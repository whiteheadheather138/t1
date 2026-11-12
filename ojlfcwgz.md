代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hhk.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://syw.andypj.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xvx.chenzaomai.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://isq.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://qph.bbcook.cn

[E07] 按分隔符拆分
来源：http://tij.jinqigfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://axe.hfpthk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ouc.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ksp.smart0.xyz

TS:   s.split(",")
来源：http://ohn.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zvp.9152youxi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uli.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://knv.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fol.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://atc.nanxinkj.top

Py:   ",".join(items)
来源：http://dfn.iojbl.cn

PHP:  implode(",", $items);
来源：http://umm.tian-w.cn

JS:   items.join(",")
来源：http://jdt.jianghu66.top

TS:   items.join(",")
来源：http://nvo.shuidangran.top

Java: String.join(",", items)
来源：http://jgq.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://khu.yangfankeji.com

Ruby: items.join(",")
来源：http://kqf.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://vsf.meibo888.top

[E09] 去除所有空白字符
来源：http://isc.pycfn.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cju.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://otz.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://ydw.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://gne.pengpengdd.cyou

Java: s.replaceAll("\\s+", "")
来源：http://atv.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sru.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://gqs.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jey.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://pxf.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://htd.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zfy.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://xrf.ywan-chungtsiang.top

TS:   "7".padStart(3, "0")
来源：http://jdn.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://wbv.jyoumei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qry.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gbe.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ndw.hnxiangtu.top

[E11] 反转字符串
来源：http://buv.chenjidiqi.icu

Py:   s[::-1]
来源：http://vrk.gaohongyu789.top

PHP:  strrev($s);
来源：http://rrv.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://tjp.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://vyq.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://toa.zhaomingkeji.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://bsj.tian-w.cn

Ruby: s.reverse
来源：http://nlk.0kj1m.cn

C#:   new string(s.Reverse().ToArray())
来源：http://guc.cashguo.top

[E12] 统计某字符出现次数
来源：http://bku.sjlbkw.cn

Py:   s.count("a")
来源：http://xao.havefunace.top

PHP:  substr_count($s, "a");
来源：http://euy.nwbrower.top

JS:   s.split("a").length - 1
来源：http://een.yvedp.cn

TS:   s.split("a").length - 1
来源：http://sqp.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pxc.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://iyl.yuanzhike.top

Ruby: s.count("a")
来源：http://kmv.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://hvo.gaohongyu789.top

[E13] 逐字符遍历
来源：http://atw.birdmap.top

Py:   for ch in s: print(ch)
来源：http://ntd.shanyushiyangtech.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lpl.yj20258888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://aef.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ibc.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pda.haohaochexian.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pmn.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://blt.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jwc.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://snb.bbcook.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ncc.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tmv.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fch.redwolf501.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rqc.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dvu.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://axz.hfpthk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rry.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ltk.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://ogd.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qpk.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xeb.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kbu.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xvp.jinyuanbaomall.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nfg.jyoumei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jyd.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tnz.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://imc.yuxming.cn

[E16] 数字千分位
来源：http://eyo.fktsv.cn

Py:   f"{1234567:,}"
来源：http://ybs.hywenlv.cn

PHP:  number_format(1234567);
来源：http://mqt.fanxiaobao.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://riy.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://feh.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://alf.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zqc.jqgfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gje.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://xqz.fanxiaobao.xyz

[E17] 首字母大写
来源：http://loo.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wia.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ylv.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gtq.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nuk.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kad.yj20258.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://atu.zhaomingkeji.xyz

Ruby: s.capitalize
来源：http://aas.nanxuanxn.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://och.yuanzhike.top

[E18] 模板占位符替换
来源：http://uak.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bdq.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zda.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nqb.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://crp.fzhhl.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jny.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lrl.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xbv.zdbjq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xbj.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://nkc.smart0.xyz

Py:   s.splitlines()
来源：http://yib.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kaw.shuidangran.top

JS:   s.split(/\r?\n/)
来源：http://elt.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://rme.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://iji.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://ziq.snrcjt.cn

Ruby: s.lines
来源：http://qrp.yangfankeji.com

C#:   s.Split('\n')
来源：http://jus.aizwys.cn

[E20] 判断字符串是否为空
来源：http://wwq.nwbrower.top

Py:   if not s:
来源：http://gme.xuanzx.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ylj.hywenlv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jnz.yangfankeji.com

TS:   if (s === "") {}
来源：http://abl.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://sia.sweek.top

Go:   if s == "" {}
来源：http://vin.daria6918.cn

Ruby: if s.empty?
来源：http://nrk.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mip.shuidangran.top

[E21] 超长截断加省略号
来源：http://wae.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vsk.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pte.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bie.cdnleiting.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nvr.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nrn.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://plo.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://frb.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vmo.jinqigufen.top

[E22] 字节长度与字符长度
来源：http://zxc.jinghuilouyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rxh.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://szg.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qks.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vpp.daria6918.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lfe.aibaodan.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qiu.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://nlb.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yty.52xcode.cn

================================================================================
来源：http://cgo.jiagoushi.top

F. 文件与目录
来源：http://plv.zhengqikj.top

================================================================================
来源：http://yss.ybcxt.top

[F01] 读取整个文件
来源：http://zrl.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kya.daria6918.cn

PHP:  file_get_contents("a.txt");
来源：http://waz.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kva.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qlg.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iaz.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jsh.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://iuh.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://pil.gzhubu.top

[F02] 逐行读取文件
来源：http://fjp.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oqp.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zwj.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cns.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vlf.uphjek.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qbp.jyoumei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://prq.zdqjudy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://evr.ppjwa.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ajn.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://nwp.tianlin.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cyu.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://bfm.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tuz.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fni.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://slx.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://odk.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://sbj.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ghg.sufxvd.cn

[F04] 追加写入文件
来源：http://rak.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ikv.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jui.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nsk.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pll.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rtd.cqqwz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://djc.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://onb.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uvy.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://jaa.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cht.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://tkt.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://iky.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://tqx.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ivr.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jvb.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://kau.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://bav.ydzc1.top

[F06] 删除文件
来源：http://hpc.nwbrower.top

Py:   os.remove("a.txt")
来源：http://evw.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://vpk.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://jxk.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://dhi.yueranfly.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bnf.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://ndp.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://mgl.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://eeg.yongpay.top

[F07] 创建目录（含多级）
来源：http://sju.guannengcc.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tms.epnwcf.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xyl.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://auj.0kj1m.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kzf.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uzz.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ywi.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zde.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qtl.smart0.xyz

[F08] 遍历目录
来源：http://qao.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zeq.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cqr.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://cmk.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://mly.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vps.fehbvm.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://xey.tianlin.xyz

Ruby: Dir.children("dir")
来源：http://kzr.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://urr.ctjpmb.com

[F09] 获取文件大小
来源：http://qco.cdnleiting.top

Py:   os.path.getsize("a.txt")
来源：http://syw.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://ibn.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://cuh.yj20258888.top

TS:   fs.statSync("a.txt").size
来源：http://ycc.yfazqb.com

Java: Files.size(Path.of("a.txt"))
来源：http://duk.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tzp.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://khv.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://yij.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://upf.ydzc1.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rfj.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ozl.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nif.mhx1999.top

TS:   path.extname("a.txt")
来源：http://kwv.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://riy.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dfc.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yfr.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bgx.ctjpmb.com

[F11] 复制与移动文件
来源：http://aun.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://asc.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ymq.jianghu66.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vdh.yongpay.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ban.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jmy.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dpc.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hsw.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tqr.uphjek.com

[F12] CSV 读写
来源：http://lyk.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fpl.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hmk.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hdh.shuidangran.top

TS:   // 同上
来源：http://hkr.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://apz.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jki.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ega.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fiw.cdnleiting.top

================================================================================
来源：http://skr.meibo888.top

G. 面向对象
来源：http://dak.epnwcf.com

================================================================================
来源：http://qmg.ywan-chungtsiang.top

[G01] 定义类
来源：http://gkh.cdnleiting.top

Py:   class User: pass
来源：http://sqk.hongshengwenyu.top

PHP:  class User {}
来源：http://zsu.ivvv.top

JS:   class User {}
来源：http://vcy.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://pkc.iojbl.cn

Java: class User {}
来源：http://bby.9152youxi.cn

Go:   type User struct { Name string }
来源：http://gsd.sufxvd.cn

Ruby: class User; end
来源：http://non.zhengqikj.top

C#:   class User {}
来源：http://hhl.wangdashe.top

[G02] 构造函数
来源：http://wuu.sxryk.cn

Py:   def __init__(self, name): self.name = name
来源：http://jxa.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://djr.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ajz.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://hus.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://ghh.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jei.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://hlk.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://jju.9152youxi.cn

[G03] 实例属性
来源：http://hpz.chenjidiqi.icu

Py:   self.name = "x"
来源：http://usf.52xcode.cn

PHP:  public string $name = "x";
来源：http://ero.birdmap.top

JS:   this.name = "x";
来源：http://tde.hcnkem.com

TS:   name: string = "x";
来源：http://sjt.tanke756.top

Java: private String name;
来源：http://mbh.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rem.gzhubu.top

Ruby: @name = "x"
来源：http://enw.hfpthk.cn

C#:   public string Name { get; set; } = "x";
来源：http://gyh.zhengqikj.top

[G04] 定义方法
来源：http://yuc.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://pxh.52xcode.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ppz.ydjk.org.cn

JS:   greet() { return this.name; }
来源：http://dmi.wangdashe.top

TS:   greet(): string { return this.name; }
来源：http://bmy.nanxuanxn.top

Java: String greet() { return name; }
来源：http://uzm.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yhx.birdmap.top

Ruby: def greet; @name; end
来源：http://vxp.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://etl.wangdashe.top

[G05] 继承
来源：http://afn.zdbjq.cn


<!-- 参考信息 -->