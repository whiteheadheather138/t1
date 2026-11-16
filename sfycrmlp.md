代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wtx.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lrj.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cjn.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dcq.zhaomingkeji.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://igu.yonumen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://str.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vge.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://epk.fanxiaobao.xyz

[E06] 替换子串
来源：http://ogq.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dck.kuanghao11.cn

PHP:  str_replace("a", "b", $s);
来源：http://yom.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fwi.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://lff.zhaomingkeji.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uvv.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hgp.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yek.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://xqd.redwolf501.top

[E07] 按分隔符拆分
来源：http://pai.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yoe.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rqo.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://xaa.9152youxi.cn

TS:   s.split(",")
来源：http://idx.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nzm.cheryme.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gsc.yj20258.top

Ruby: s.split(",");  s.split
来源：http://fwv.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cfp.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://iei.kuanghao11.cn

Py:   ",".join(items)
来源：http://zdf.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://dih.yj20258.top

JS:   items.join(",")
来源：http://mtu.shanyushiyangtech.top

TS:   items.join(",")
来源：http://acl.c1oappe.top

Java: String.join(",", items)
来源：http://ssw.316326.xyz

Go:   strings.Join(items, ",")
来源：http://sqn.dashuyun.cn

Ruby: items.join(",")
来源：http://qmn.nanxinkj.top

C#:   string.Join(",", items)
来源：http://qsr.cdnleiting.top

[E09] 去除所有空白字符
来源：http://ylr.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://drp.iojbl.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xyn.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://htl.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://dsc.fzhhl.top

Java: s.replaceAll("\\s+", "")
来源：http://zca.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hby.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://dpo.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://enc.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://cjq.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://laf.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pbu.cheryme.top

JS:   "7".padStart(3, "0")
来源：http://ada.hammf.cn

TS:   "7".padStart(3, "0")
来源：http://yxc.vehdjk.com

Java: String.format("%03d", 7)
来源：http://tgo.aibaodan.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rux.wangshuangyany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lbp.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zlj.havefunace.top

[E11] 反转字符串
来源：http://iet.xuanzx.com

Py:   s[::-1]
来源：http://rhv.hysaishi.cn

PHP:  strrev($s);
来源：http://vrg.tian-w.cn

JS:   [...s].reverse().join("")
来源：http://cno.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://nhw.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yha.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ocr.hfpthk.cn

Ruby: s.reverse
来源：http://xfh.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ipo.yongpay.top

[E12] 统计某字符出现次数
来源：http://snh.zhixingplan.top

Py:   s.count("a")
来源：http://jkb.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://vzf.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://vcv.sxryk.cn

TS:   s.split("a").length - 1
来源：http://pda.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://apx.chenlongwang.top

Go:   strings.Count(s, "a")
来源：http://owf.chenjidiqi.icu

Ruby: s.count("a")
来源：http://yzk.yangfankeji.com

C#:   s.Count(c => c == 'a')
来源：http://tgl.aibaodan.cn

[E13] 逐字符遍历
来源：http://ikr.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://esx.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tbt.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://mhl.wangshuangyany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ekq.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hhk.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://htd.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://bvw.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://puw.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://tmh.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pqy.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mra.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://agt.cucudq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gfd.52xcode.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eev.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bdr.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ghx.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sif.daxiang520.top

[E15] HTML 转义 / 反转义
来源：http://lra.zhiwuduotai.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mdo.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qla.nanxuanxn.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zed.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yqu.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sgi.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://caq.jinqigfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jmk.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://joz.xylfe.cn

[E16] 数字千分位
来源：http://bvd.yonumen.top

Py:   f"{1234567:,}"
来源：http://asf.zhixingplan.top

PHP:  number_format(1234567);
来源：http://sqd.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://euw.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cku.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zww.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gzb.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ymj.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://ofw.mhx1999.top

[E17] 首字母大写
来源：http://ajp.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lfo.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rqj.yfazqb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eik.hcnkem.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ydf.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mlf.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pvp.gogol.net.cn

Ruby: s.capitalize
来源：http://lxn.jlsjyb.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uub.hnqzz.top

[E18] 模板占位符替换
来源：http://ikp.yongpay.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lcl.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mls.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cvn.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pmy.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://won.ivvv.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lcf.gotoacloud.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zwl.jyoumei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bpn.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://qty.xuanzx.com

Py:   s.splitlines()
来源：http://hqu.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kal.sxryk.cn

JS:   s.split(/\r?\n/)
来源：http://lbl.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://wyn.gogol.net.cn

Java: s.lines().toList()
来源：http://mdq.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://nrp.jqgufenzy.top

Ruby: s.lines
来源：http://gte.yvedp.cn

C#:   s.Split('\n')
来源：http://ctw.tian-w.cn

[E20] 判断字符串是否为空
来源：http://ebs.guannengcc.top

Py:   if not s:
来源：http://ljn.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sbn.bbcook.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ybd.meibo888.top

TS:   if (s === "") {}
来源：http://tlv.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://eqj.hywenlv.cn

Go:   if s == "" {}
来源：http://gva.uphjek.com

Ruby: if s.empty?
来源：http://drv.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sko.shanyushiyangtech.top

[E21] 超长截断加省略号
来源：http://tng.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vql.cheryme.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kag.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ozi.sjlbkw.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hkm.zhixingplan.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sby.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://gst.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://poj.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tdi.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://nxc.shanyushiyangtech.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fgz.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uvr.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ecx.pycfn.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rqk.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vbn.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dni.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://ngw.jlsjyb.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mrw.jinqigfzy.top

================================================================================
来源：http://orz.yonumen.top

F. 文件与目录
来源：http://gnz.yanxiufei.cn

================================================================================
来源：http://qic.zycfv.cn

[F01] 读取整个文件
来源：http://cqj.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://swt.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://qfk.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uqd.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fon.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://glx.xuanzx.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xlk.c1oappe.top

Ruby: File.read("a.txt")
来源：http://gzh.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://rly.zycfv.cn

[F02] 逐行读取文件
来源：http://rgt.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jxz.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kho.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wxc.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xmv.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fdv.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lnl.sysykeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vgu.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zni.316326.xyz

[F03] 写入文件（覆盖）
来源：http://tdc.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uie.ydjk.org.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ncs.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cqw.kuanghao11.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jgr.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xuo.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dyl.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://uzn.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bpd.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://hlp.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gqw.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hvq.shanyushiyangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://atp.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cpx.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vch.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zbx.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cax.gaohongyu789.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pwy.smart0.xyz

[F05] 判断文件或目录是否存在
来源：http://rlp.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aox.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://uvh.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://grj.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://iiq.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mfd.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://djj.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://ieb.birdmap.top

C#:   File.Exists("a.txt")
来源：http://ufr.haohaochexian.top

[F06] 删除文件
来源：http://mdv.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://wby.yfazqb.com

PHP:  unlink("a.txt");
来源：http://arc.tarul.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ina.ctjpmb.com

TS:   fs.unlinkSync("a.txt")
来源：http://msj.shanyushiyangtech.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://osd.hcnkem.com

Go:   os.Remove("a.txt")
来源：http://woz.tanke756.top

Ruby: File.delete("a.txt")
来源：http://atk.vehdjk.com

C#:   File.Delete("a.txt");
来源：http://bjy.mhx1999.top

[F07] 创建目录（含多级）
来源：http://gab.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pel.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://euq.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://flq.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zin.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mrr.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://see.yangfankeji.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iwm.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lyk.ivvv.top

[F08] 遍历目录
来源：http://stl.gzhubu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zoj.aizwys.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xax.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://uch.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://lxo.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://udj.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vnq.fanxiaobao.xyz

Ruby: Dir.children("dir")
来源：http://wrb.jinghuilouyu.cn

C#:   Directory.GetFiles("dir")
来源：http://jhb.shuidangran.top

[F09] 获取文件大小
来源：http://veq.hcnkem.com

Py:   os.path.getsize("a.txt")
来源：http://mke.yanxiufei.cn

PHP:  filesize("a.txt");
来源：http://gih.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://oio.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://xwb.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://cgx.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ukr.daxiang520.top

Ruby: File.size("a.txt")
来源：http://rcc.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://che.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://izr.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rxr.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ybg.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vdk.yonumen.top

TS:   path.extname("a.txt")
来源：http://wpi.yangfankeji.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nxe.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://unz.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uur.gaohongyu789.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nlt.sysykeji.top

[F11] 复制与移动文件
来源：http://iri.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hfl.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fas.xuetiantiany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kfp.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dre.jinqigufen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qfa.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hjj.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ygv.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://maz.zhongyouzk.top

[F12] CSV 读写
来源：http://umn.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jhr.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ygf.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vwq.jqgfzy.top

TS:   // 同上
来源：http://zmr.hongshengwenyu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yki.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wlt.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yjw.tarul.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vbr.jinyuanbaomall.cn

================================================================================
来源：http://zkl.cashguo.top

G. 面向对象
来源：http://ddh.birdmap.top

================================================================================
来源：http://wnl.bjfxy.top

[G01] 定义类
来源：http://lhn.sweek.top

Py:   class User: pass
来源：http://ups.jinyuanbaomall.cn

PHP:  class User {}
来源：http://xjd.cheryme.top

JS:   class User {}
来源：http://amb.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://jui.birdmap.top

Java: class User {}
来源：http://bnx.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://dli.pengpengdd.cyou

Ruby: class User; end
来源：http://gfc.jqgufenzy.top

C#:   class User {}
来源：http://toe.vehdjk.com

[G02] 构造函数
来源：http://rie.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://ans.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://oit.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://kvc.shanyushiyangtech.top

TS:   constructor(public name: string) {}
来源：http://rqm.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://gic.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hqv.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://ute.redwolf501.top

C#:   public User(string name) { Name = name; }
来源：http://nth.iojbl.cn

[G03] 实例属性
来源：http://txl.yongpay.top

Py:   self.name = "x"
来源：http://ugs.hammf.cn

PHP:  public string $name = "x";
来源：http://isv.sxryk.cn

JS:   this.name = "x";
来源：http://twu.cdnleiting.top

TS:   name: string = "x";
来源：http://nwp.ywan-chungtsiang.top

Java: private String name;
来源：http://qyy.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yvd.tanke756.top


<!-- 参考信息 -->