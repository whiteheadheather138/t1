代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xvh.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sbk.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ziv.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://imc.0kj1m.cn

[E06] 替换子串
来源：http://sma.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vmu.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://mna.bjfxy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ymv.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://yxv.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bfs.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lof.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vza.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://cuy.iojbl.cn

[E07] 按分隔符拆分
来源：http://xwe.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://abh.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uip.hywenlv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kzc.jlsjyb.cn

TS:   s.split(",")
来源：http://xzj.xingfuxueyuan.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://jyb.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hdd.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://rjy.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://war.svipenyu.cn

[E08] 数组按分隔符合并
来源：http://bal.fengsongda.top

Py:   ",".join(items)
来源：http://mwq.tian-w.cn

PHP:  implode(",", $items);
来源：http://ipa.ydzc1.top

JS:   items.join(",")
来源：http://gdm.meibo888.top

TS:   items.join(",")
来源：http://ecd.smart0.xyz

Java: String.join(",", items)
来源：http://ged.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://cpe.jiagoushi.top

Ruby: items.join(",")
来源：http://maz.shuidangran.top

C#:   string.Join(",", items)
来源：http://ktd.hesvh.cn

[E09] 去除所有空白字符
来源：http://srj.c1oappe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iko.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rou.feifeiyinyue.top

JS:   s.replace(/\s+/g, "")
来源：http://xot.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://rnu.ctjpmb.com

Java: s.replaceAll("\\s+", "")
来源：http://wzz.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wnt.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wmm.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dqy.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://zag.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yhd.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://odr.yuanzhike.top

JS:   "7".padStart(3, "0")
来源：http://szv.daria6918.cn

TS:   "7".padStart(3, "0")
来源：http://dki.cheryme.top

Java: String.format("%03d", 7)
来源：http://lrr.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://syz.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fel.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qlc.snrcjt.cn

[E11] 反转字符串
来源：http://jop.sweek.top

Py:   s[::-1]
来源：http://qnq.snrcjt.cn

PHP:  strrev($s);
来源：http://gev.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://quy.tanke756.top

TS:   [...s].reverse().join("")
来源：http://abp.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://owd.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vpv.yuanzhike.top

Ruby: s.reverse
来源：http://llz.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tsi.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://fkk.nwbrower.top

Py:   s.count("a")
来源：http://axw.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://bfd.sweek.top

JS:   s.split("a").length - 1
来源：http://rka.yanxiufei.cn

TS:   s.split("a").length - 1
来源：http://uiu.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iws.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://kyz.shzxlz.cn

Ruby: s.count("a")
来源：http://uum.yvedp.cn

C#:   s.Count(c => c == 'a')
来源：http://pwn.jinqigfzy.top

[E13] 逐字符遍历
来源：http://eco.sjlbkw.cn

Py:   for ch in s: print(ch)
来源：http://afz.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://beo.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lco.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ktk.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cka.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jyo.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dlo.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ond.xylfe.cn

[E14] URL 编码与 Base64
来源：http://xsm.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zmt.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mta.nwbrower.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gry.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kxv.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xbi.zdbjq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ddt.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dau.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://psk.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://uik.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zwz.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pdy.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bom.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ftk.hnqzz.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mcm.tianlin.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yxv.hnxiangtu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yvn.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tbm.snrcjt.cn

[E16] 数字千分位
来源：http://oon.pycfn.com

Py:   f"{1234567:,}"
来源：http://rbv.gotoacloud.top

PHP:  number_format(1234567);
来源：http://vhw.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://glq.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://knz.jqgfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://avy.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ure.chenzaomai.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fkf.jinqigufen.top

C#:   1234567.ToString("N0")
来源：http://vez.cheryme.top

[E17] 首字母大写
来源：http://qgv.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cxb.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xoj.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xhv.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://thl.pycfn.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ljl.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zbj.hfpthk.cn

Ruby: s.capitalize
来源：http://jue.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fvz.cqqwz.cn

[E18] 模板占位符替换
来源：http://qfs.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qie.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nwc.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://xgk.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://alw.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iwe.ehwqpu.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hwn.jqgufenzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kar.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hyg.yueranfly.top

[E19] 多行文本按行拆分
来源：http://upr.jinqigfzy.top

Py:   s.splitlines()
来源：http://ziu.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xrh.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://psn.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://gig.xingfuxueyuan.xyz

Java: s.lines().toList()
来源：http://byn.gzhubu.top

Go:   strings.Split(s, "\n")
来源：http://clq.yonumen.top

Ruby: s.lines
来源：http://usu.gzhubu.top

C#:   s.Split('\n')
来源：http://mfj.yongpay.top

[E20] 判断字符串是否为空
来源：http://wsz.havefunace.top

Py:   if not s:
来源：http://dzo.zhiwuduotai.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bmk.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ocd.yj20258888.top

TS:   if (s === "") {}
来源：http://sep.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://lto.tanke756.top

Go:   if s == "" {}
来源：http://opi.yvedp.cn

Ruby: if s.empty?
来源：http://uqi.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dwb.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://knc.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bxl.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uml.jinqigfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fdx.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qnb.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://auv.ppjwa.cn

Go:   // 按 rune 判断长度后截断
来源：http://bch.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ugw.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kpv.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://siy.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://plj.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cve.birdmap.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://puh.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://apl.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lbi.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iod.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://bwg.yanxiufei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rko.jinqigufen.top

================================================================================
来源：http://rnm.9152youxi.cn

F. 文件与目录
来源：http://dmy.hysaishi.cn

================================================================================
来源：http://qxr.cdnleiting.top

[F01] 读取整个文件
来源：http://iqd.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://goh.sysykeji.top

PHP:  file_get_contents("a.txt");
来源：http://dcb.yongpay.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kqe.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kil.zhongyouzk.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xfd.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zkb.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://fom.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://chk.zdbjq.cn

[F02] 逐行读取文件
来源：http://ulz.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vca.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kko.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hoi.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pwv.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zbn.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kfn.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ldm.xziqi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dbf.fanxiaobao.xyz

[F03] 写入文件（覆盖）
来源：http://edi.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pjs.tarul.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qcr.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://seq.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bmt.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sfk.chenzaomai.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ogv.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://frl.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nah.jqgufenzy.top

[F04] 追加写入文件
来源：http://djt.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oyd.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tiy.svipenyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lex.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ubo.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ixp.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eqb.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yiz.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://flr.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://uby.wangdashe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xem.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://njg.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://hvj.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://gdj.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://unf.chenlongwang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cmg.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://gov.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://cpv.redwolf501.top

[F06] 删除文件
来源：http://xdh.aizwys.cn

Py:   os.remove("a.txt")
来源：http://qwh.vqdsnc.cn

PHP:  unlink("a.txt");
来源：http://ikt.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://osm.ctjpmb.com

TS:   fs.unlinkSync("a.txt")
来源：http://swc.zhiwuduotai.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ndi.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://ife.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://fdc.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://lzi.yueranfly.top

[F07] 创建目录（含多级）
来源：http://fim.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rhd.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cii.hongshengwenyu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bkz.mhx1999.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tzu.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lhj.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://buf.xuanzx.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bdn.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dui.jqgufenzy.top

[F08] 遍历目录
来源：http://hnw.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://gno.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vfb.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://ftx.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://fzr.gzhubu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uaq.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rzp.daria6918.cn

Ruby: Dir.children("dir")
来源：http://ipq.zhaomingkeji.xyz

C#:   Directory.GetFiles("dir")
来源：http://sqv.nwbrower.top

[F09] 获取文件大小
来源：http://btr.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://fgo.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://zrt.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://egb.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://rwz.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://wsz.fanxiaobao.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mqf.wangdashe.top

Ruby: File.size("a.txt")
来源：http://sda.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://wkk.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://gvs.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aie.yj202588.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qru.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nwq.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://two.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dzm.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tyf.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wsw.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://glr.ivvv.top

[F11] 复制与移动文件
来源：http://emt.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zwo.yvedp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yhk.bbcook.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://khu.epnwcf.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xts.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kza.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://owg.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tow.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ylf.yfazqb.com

[F12] CSV 读写
来源：http://klr.havefunace.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ayh.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://phw.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://esm.gotoacloud.top

TS:   // 同上
来源：http://mzq.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rhi.52xcode.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xlf.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vqd.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wfx.nanxinkj.top

================================================================================
来源：http://kkr.52xcode.cn

G. 面向对象
来源：http://qzz.pengpengdd.cyou

================================================================================
来源：http://pwq.havefunace.top

[G01] 定义类
来源：http://xub.guowangkeji.top

Py:   class User: pass
来源：http://tft.aizwys.cn

PHP:  class User {}
来源：http://tfx.yj20258.top

JS:   class User {}
来源：http://ywf.sweek.top

TS:   class User { name: string = ""; }
来源：http://cxs.zhixingplan.top

Java: class User {}
来源：http://hdw.52xcode.cn

Go:   type User struct { Name string }
来源：http://yoc.cdnleiting.top

Ruby: class User; end
来源：http://gek.andypj.xyz

C#:   class User {}
来源：http://ktr.zhoulong.xyz

[G02] 构造函数
来源：http://psr.snrcjt.cn

Py:   def __init__(self, name): self.name = name
来源：http://mge.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://hzv.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://zoo.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://eak.mhx1999.top

Java: User(String name) { this.name = name; }
来源：http://pra.jianghu66.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://suy.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ezf.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://yot.wangshuangyany.cn

[G03] 实例属性
来源：http://wni.meibo888.top

Py:   self.name = "x"
来源：http://gtk.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://tiy.xuanzx.com

JS:   this.name = "x";
来源：http://xeb.zycfv.cn

TS:   name: string = "x";
来源：http://kdv.0kj1m.cn

Java: private String name;
来源：http://eaj.xingfuxueyuan.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wom.0kj1m.cn

Ruby: @name = "x"
来源：http://uxp.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://pom.hesvh.cn

[G04] 定义方法
来源：http://wgp.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://szn.xziqi.cn


<!-- 参考信息 -->