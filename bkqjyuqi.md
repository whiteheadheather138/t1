代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qqg.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ern.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nwx.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://msj.yvedp.cn

[E06] 替换子串
来源：http://xph.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ggh.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://qbq.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vnv.dashuyun.cn

TS:   s.replaceAll("a", "b")
来源：http://hms.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eko.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gtc.vqdsnc.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jvz.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://mlp.yueranfly.top

[E07] 按分隔符拆分
来源：http://rot.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wrz.xuetiantiany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wcd.jinqigufen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iba.zycfv.cn

TS:   s.split(",")
来源：http://vhk.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://kdq.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iae.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://zxo.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://isr.ivvv.top

[E08] 数组按分隔符合并
来源：http://vnm.hywenlv.cn

Py:   ",".join(items)
来源：http://frl.fzhhl.top

PHP:  implode(",", $items);
来源：http://pre.tanke756.top

JS:   items.join(",")
来源：http://neh.nanxuanxn.top

TS:   items.join(",")
来源：http://hbl.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://rsf.havefunace.top

Go:   strings.Join(items, ",")
来源：http://hiy.sweek.top

Ruby: items.join(",")
来源：http://sfj.yj20258.top

C#:   string.Join(",", items)
来源：http://fdl.fzhhl.top

[E09] 去除所有空白字符
来源：http://vzz.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bwm.jqgfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xye.yongpay.top

JS:   s.replace(/\s+/g, "")
来源：http://nqq.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://tqv.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://goh.dashuyun.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://itz.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://srj.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oyx.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://vsh.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dlj.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vce.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://kjc.9152youxi.cn

TS:   "7".padStart(3, "0")
来源：http://gwj.fktsv.cn

Java: String.format("%03d", 7)
来源：http://vlj.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jcq.cheryme.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tlz.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qiq.ctjpmb.com

[E11] 反转字符串
来源：http://osc.zdbjq.cn

Py:   s[::-1]
来源：http://bcp.tian-w.cn

PHP:  strrev($s);
来源：http://ewq.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://aip.yuxming.cn

TS:   [...s].reverse().join("")
来源：http://rwl.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://axv.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uce.shzxlz.cn

Ruby: s.reverse
来源：http://csj.hammf.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ghv.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://qwb.gaohongyu789.top

Py:   s.count("a")
来源：http://nsm.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://nci.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://vgk.hammf.cn

TS:   s.split("a").length - 1
来源：http://frk.xinyue.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ifw.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://cls.snrcjt.cn

Ruby: s.count("a")
来源：http://jeh.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://gaj.xziqi.cn

[E13] 逐字符遍历
来源：http://hdg.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://lvq.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fvs.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ykz.fanxiaobao.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://seo.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bqa.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zrx.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://piw.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vpe.hammf.cn

[E14] URL 编码与 Base64
来源：http://xuk.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jud.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tas.gaohongyu789.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tfr.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yla.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cxm.sufxvd.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gbs.bbcook.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rfw.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kvh.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://uge.yanxiufei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nqr.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xxd.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tml.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ddb.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zoq.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://otq.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ual.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nbe.dashuyun.cn

[E16] 数字千分位
来源：http://wsq.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://qdn.mhx1999.top

PHP:  number_format(1234567);
来源：http://wmw.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qmk.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ahc.pycfn.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://laq.yj20258888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rnc.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fyr.daria6918.cn

C#:   1234567.ToString("N0")
来源：http://vjz.yj20258888.top

[E17] 首字母大写
来源：http://xfu.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://btm.jiagoushi.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dkb.yfazqb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bpo.pengpengdd.cyou

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zig.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ult.yvedp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ymg.hywenlv.cn

Ruby: s.capitalize
来源：http://avr.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hzf.jinghuilouyu.cn

[E18] 模板占位符替换
来源：http://tms.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kxl.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://smz.nanxuanxn.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jbk.zhongyouzk.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lil.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jwe.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ggq.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rjf.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ung.zycfv.cn

[E19] 多行文本按行拆分
来源：http://mba.yuxming.cn

Py:   s.splitlines()
来源：http://ayl.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zfe.hcnkem.com

JS:   s.split(/\r?\n/)
来源：http://xoe.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://jer.ehwqpu.com

Java: s.lines().toList()
来源：http://eaa.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://rnb.yj20258888.top

Ruby: s.lines
来源：http://yvy.fktsv.cn

C#:   s.Split('\n')
来源：http://azs.ybcxt.top

[E20] 判断字符串是否为空
来源：http://edk.bjfxy.top

Py:   if not s:
来源：http://zrc.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ghm.hcnkem.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bju.hongshengwenyu.top

TS:   if (s === "") {}
来源：http://vle.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://its.ivvv.top

Go:   if s == "" {}
来源：http://vfz.guowangkeji.top

Ruby: if s.empty?
来源：http://wde.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rvf.aizwys.cn

[E21] 超长截断加省略号
来源：http://iet.hfpthk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kia.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vwf.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://utn.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yes.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lyb.fanxiaobao.xyz

Go:   // 按 rune 判断长度后截断
来源：http://fpl.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kvn.jyoumei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tvp.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://kkw.mhx1999.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nqh.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jas.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wvc.zhoulong.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sti.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://afn.aibaodan.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dqv.hnxiangtu.top

Ruby: s.bytesize;  s.length
来源：http://gpt.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nhw.sjlbkw.cn

================================================================================
来源：http://xpj.xinyue.icu

F. 文件与目录
来源：http://fvk.jianghu66.top

================================================================================
来源：http://jbz.zdbjq.cn

[F01] 读取整个文件
来源：http://fax.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sme.daria6918.cn

PHP:  file_get_contents("a.txt");
来源：http://lue.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qwg.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vcq.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dxt.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kqc.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://ipj.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://bzs.bbcook.cn

[F02] 逐行读取文件
来源：http://jqg.yuxming.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qnt.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://azv.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://anx.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cxd.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kmx.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://clc.chenlongwang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xjt.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wgr.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://rkw.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://udr.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xiw.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cqq.yuanzhike.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ody.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xti.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cgp.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://nmj.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://enr.hywenlv.cn

[F04] 追加写入文件
来源：http://iqw.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xnw.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vws.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jik.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qiw.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wsc.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://psj.316326.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bzx.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sia.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://gii.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mfa.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://dkc.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://ghm.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://uas.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yxn.yj20258888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fdh.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://bmu.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://hau.xylfe.cn

[F06] 删除文件
来源：http://moy.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://lgi.yuanzhike.top

PHP:  unlink("a.txt");
来源：http://uao.zhixingplan.top

JS:   fs.unlinkSync("a.txt")
来源：http://fkn.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sgl.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bza.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://hjr.316326.xyz

Ruby: File.delete("a.txt")
来源：http://tfw.aibaodan.cn

C#:   File.Delete("a.txt");
来源：http://ygl.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://tmh.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cbk.yuxming.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rgb.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jjq.sufxvd.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fsh.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://odz.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://myt.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qyq.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://srw.sufxvd.cn

[F08] 遍历目录
来源：http://dtp.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jmg.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kys.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://fuv.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://wdm.c1oappe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ptg.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zwq.xziqi.cn

Ruby: Dir.children("dir")
来源：http://fnc.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://wic.jlsjyb.cn

[F09] 获取文件大小
来源：http://dls.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://zes.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://cpd.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://wmk.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://rpc.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://pvt.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zjv.xinyue.icu

Ruby: File.size("a.txt")
来源：http://wtl.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://nsr.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://asf.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mbd.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dop.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qtg.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://blr.guowangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xqo.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sot.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://npc.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rxs.c1oappe.top

[F11] 复制与移动文件
来源：http://hlx.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wzh.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qyl.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vlc.daxiang520.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tpa.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tmf.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wtb.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yjq.snrcjt.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://prb.cqqwz.cn

[F12] CSV 读写
来源：http://ahd.cucudq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uhk.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fmt.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rax.ivvv.top

TS:   // 同上
来源：http://hne.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://thx.snrcjt.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zwf.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cey.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qvw.xuanzx.com

================================================================================
来源：http://faw.sufxvd.cn

G. 面向对象
来源：http://gwq.chenlongwang.top

================================================================================
来源：http://fwr.feifeiyinyue.top

[G01] 定义类
来源：http://otj.yvedp.cn

Py:   class User: pass
来源：http://txh.sjlbkw.cn

PHP:  class User {}
来源：http://xbv.shzxlz.cn

JS:   class User {}
来源：http://vdf.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://uxs.sysykeji.top

Java: class User {}
来源：http://ojf.jianghu66.top

Go:   type User struct { Name string }
来源：http://vnm.chenlongwang.top

Ruby: class User; end
来源：http://bgf.sysykeji.top

C#:   class User {}
来源：http://hqc.bjfxy.top

[G02] 构造函数
来源：http://let.xziqi.cn

Py:   def __init__(self, name): self.name = name
来源：http://itp.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://nvq.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://fnl.tanke756.top

TS:   constructor(public name: string) {}
来源：http://xns.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://kxm.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uyc.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://izr.bbcook.cn

C#:   public User(string name) { Name = name; }
来源：http://apv.mhx1999.top

[G03] 实例属性
来源：http://fac.redwolf501.top

Py:   self.name = "x"
来源：http://toc.smart0.xyz

PHP:  public string $name = "x";
来源：http://ytu.xziqi.cn

JS:   this.name = "x";
来源：http://jrn.feifeiyinyue.top

TS:   name: string = "x";
来源：http://lll.uphjek.com

Java: private String name;
来源：http://nce.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ouc.xylfe.cn

Ruby: @name = "x"
来源：http://wdi.fanxiaobao.xyz

C#:   public string Name { get; set; } = "x";
来源：http://qhj.jinghuilouyu.cn

[G04] 定义方法
来源：http://zyg.hcnkem.com

Py:   def greet(self): return self.name
来源：http://vut.gaohongyu789.top


<!-- 参考信息 -->