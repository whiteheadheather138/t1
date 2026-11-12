代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rgg.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hvq.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ppe.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ygo.gogol.net.cn

[E06] 替换子串
来源：http://tnh.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cen.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://ayv.hammf.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://owq.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://etq.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jrt.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gub.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pep.birdmap.top

C#:   s.Replace("a", "b")
来源：http://jhj.quarkkingdee.top

[E07] 按分隔符拆分
来源：http://lbs.shangyingyoupin.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://idj.ivvv.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sez.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://eok.hcnkem.com

TS:   s.split(",")
来源：http://kvq.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://qbf.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://enw.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://buk.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qvg.gzhubu.top

[E08] 数组按分隔符合并
来源：http://wey.fktsv.cn

Py:   ",".join(items)
来源：http://shl.svipenyu.cn

PHP:  implode(",", $items);
来源：http://pjp.fehbvm.com

JS:   items.join(",")
来源：http://zlx.dianchejie.cn

TS:   items.join(",")
来源：http://jba.jinqigfzy.top

Java: String.join(",", items)
来源：http://uma.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://wch.pycfn.com

Ruby: items.join(",")
来源：http://kqq.tarul.cn

C#:   string.Join(",", items)
来源：http://dxn.yonumen.top

[E09] 去除所有空白字符
来源：http://ffu.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kin.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aqj.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://lpq.chenzaomai.com

TS:   s.replace(/\s+/g, "")
来源：http://srs.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://tgj.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://fhn.wangdashe.top

Ruby: s.gsub(/\s+/, "")
来源：http://lzs.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://egw.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://cek.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xxa.zhixingplan.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ani.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://brv.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://oey.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://brh.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://grp.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://buo.cheryme.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zpa.zhoulong.xyz

[E11] 反转字符串
来源：http://ndj.c1oappe.top

Py:   s[::-1]
来源：http://exk.hesvh.cn

PHP:  strrev($s);
来源：http://lfe.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://vrz.uphjek.com

TS:   [...s].reverse().join("")
来源：http://pvj.sysykeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ocs.cqqwz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pok.yongpay.top

Ruby: s.reverse
来源：http://wzr.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://xuv.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://nba.zhoulong.xyz

Py:   s.count("a")
来源：http://bgc.hongshengwenyu.top

PHP:  substr_count($s, "a");
来源：http://jxy.fengsongda.top

JS:   s.split("a").length - 1
来源：http://oku.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://fim.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bmy.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://qrd.kuanghao11.cn

Ruby: s.count("a")
来源：http://fdf.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://hxy.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://kpz.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://qxu.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nna.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://boh.gzhubu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lmb.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://czd.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://crr.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://jzm.cucudq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ijq.cucudq.cn

[E14] URL 编码与 Base64
来源：http://ysl.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jyk.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qit.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yce.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://svd.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zdd.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wud.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://juc.nwbrower.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qnb.gotoacloud.top

[E15] HTML 转义 / 反转义
来源：http://qvk.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://nlu.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wck.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sro.ehwqpu.com

TS:   // 同上，务必做 XSS 过滤
来源：http://iod.vehdjk.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iat.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wta.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vwy.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fuk.guowangkeji.top

[E16] 数字千分位
来源：http://azu.0kj1m.cn

Py:   f"{1234567:,}"
来源：http://hnw.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://onj.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vzl.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lhm.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mur.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eiv.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qaa.pycfn.com

C#:   1234567.ToString("N0")
来源：http://pys.ppjwa.cn

[E17] 首字母大写
来源：http://rzp.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zzn.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://swj.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qwz.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://egs.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://suu.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gpl.redwolf501.top

Ruby: s.capitalize
来源：http://htz.zdqjudy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gxj.jlsjyb.cn

[E18] 模板占位符替换
来源：http://xif.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yap.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qax.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tey.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jym.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vqa.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tfd.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zan.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fkf.hywenlv.cn

[E19] 多行文本按行拆分
来源：http://mky.dianchejie.cn

Py:   s.splitlines()
来源：http://hgk.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mbp.sweek.top

JS:   s.split(/\r?\n/)
来源：http://mdr.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://evu.svipenyu.cn

Java: s.lines().toList()
来源：http://lba.redwolf501.top

Go:   strings.Split(s, "\n")
来源：http://mug.wangdashe.top

Ruby: s.lines
来源：http://pxo.xuanzx.com

C#:   s.Split('\n')
来源：http://znq.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://mmp.guowangkeji.top

Py:   if not s:
来源：http://qpd.jiagoushi.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yog.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wel.fehbvm.com

TS:   if (s === "") {}
来源：http://jvt.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://gmu.0kj1m.cn

Go:   if s == "" {}
来源：http://fga.sysykeji.top

Ruby: if s.empty?
来源：http://kyl.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ijq.jqgfzy.top

[E21] 超长截断加省略号
来源：http://dzn.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vui.jinqigfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xme.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gvn.tian-w.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jnj.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xzz.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://qwj.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hif.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zpk.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://xoq.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hkc.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iaq.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://prg.yuxming.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jtb.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lfj.chenjidiqi.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hea.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://vrd.yanxiufei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vpa.xylfe.cn

================================================================================
来源：http://rde.aibaodan.cn

F. 文件与目录
来源：http://onl.bjfxy.top

================================================================================
来源：http://wsv.jiagoushi.top

[F01] 读取整个文件
来源：http://mfo.yj20258888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yxz.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://qlf.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fgx.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kue.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://arh.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kcn.daxiang520.top

Ruby: File.read("a.txt")
来源：http://sxq.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://yek.wangdashe.top

[F02] 逐行读取文件
来源：http://pmd.yangfankeji.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fgj.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://roa.sjlbkw.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cus.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fna.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kry.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zxc.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eyv.nanxuanxn.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vvu.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://nlw.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iiz.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xxp.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uix.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uhg.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xqd.hongshengwenyu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kkt.xingfuxueyuan.xyz

Ruby: File.write("a.txt", "hi")
来源：http://lzn.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vrr.yuanzhike.top

[F04] 追加写入文件
来源：http://sya.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dvb.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cqk.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://own.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cyv.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nji.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qmh.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://agf.chenlongwang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jwk.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://obj.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qze.0kj1m.cn

PHP:  file_exists("a.txt");
来源：http://kwe.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://rrg.smart0.xyz

TS:   fs.existsSync("a.txt")
来源：http://ylp.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://txn.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://klq.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://bqs.wangdashe.top

C#:   File.Exists("a.txt")
来源：http://iwa.epnwcf.com

[F06] 删除文件
来源：http://yxo.yj20258.top

Py:   os.remove("a.txt")
来源：http://drd.kuanghao11.cn

PHP:  unlink("a.txt");
来源：http://xsc.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://jcx.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://lfw.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kae.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://eaf.pycfn.com

Ruby: File.delete("a.txt")
来源：http://yyl.tianlin.xyz

C#:   File.Delete("a.txt");
来源：http://ddo.cashguo.top

[F07] 创建目录（含多级）
来源：http://ujb.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wzo.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ftq.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://itb.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yai.chenjidiqi.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qzh.andypj.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xrm.ehwqpu.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://otk.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bhs.fengsongda.top

[F08] 遍历目录
来源：http://bdr.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://eys.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pvz.xinyue.icu

JS:   fs.readdirSync("dir")
来源：http://ghc.jinqigfzy.top

TS:   fs.readdirSync("dir")
来源：http://vbc.gzhubu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ebk.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kak.nanxinkj.top

Ruby: Dir.children("dir")
来源：http://hrc.aizwys.cn

C#:   Directory.GetFiles("dir")
来源：http://xcb.yj20258.top

[F09] 获取文件大小
来源：http://yak.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://arg.gaohongyu789.top

PHP:  filesize("a.txt");
来源：http://pwc.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://yag.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://kzh.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://uqa.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tmu.cucudq.cn

Ruby: File.size("a.txt")
来源：http://asz.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://zhy.haohaochexian.top

[F10] 取文件扩展名 / 文件名
来源：http://kzv.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ltt.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yrt.hnxiangtu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tin.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://abq.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://woc.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jke.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oqc.fktsv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vxq.zhaomingkeji.xyz

[F11] 复制与移动文件
来源：http://kkf.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://adk.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ssa.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://glm.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rea.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ewv.hnqzz.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cnf.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hqd.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mxs.epnwcf.com

[F12] CSV 读写
来源：http://ejc.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://niu.pycfn.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hib.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dcs.dianchejie.cn

TS:   // 同上
来源：http://hpq.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://frz.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://scm.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pcj.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://nrr.shuidangran.top

================================================================================
来源：http://iqm.bjfxy.top

G. 面向对象
来源：http://obw.shanyushiyangkeji.top

================================================================================
来源：http://wlf.hywenlv.cn

[G01] 定义类
来源：http://glk.gaohongyu789.top

Py:   class User: pass
来源：http://alg.zycfv.cn

PHP:  class User {}
来源：http://jvm.iojbl.cn

JS:   class User {}
来源：http://rzk.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://lby.nanxuanxn.top

Java: class User {}
来源：http://xqc.hnqzz.top

Go:   type User struct { Name string }
来源：http://wrv.bjfxy.top

Ruby: class User; end
来源：http://ugc.sufxvd.cn

C#:   class User {}
来源：http://gsk.smart0.xyz

[G02] 构造函数
来源：http://gnw.fzhhl.top

Py:   def __init__(self, name): self.name = name
来源：http://mfm.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://pbl.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://pev.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://bug.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://frp.0kj1m.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nva.yj202588.top

Ruby: def initialize(name); @name = name; end
来源：http://azh.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://zog.cucudq.cn

[G03] 实例属性
来源：http://arw.ctjpmb.com

Py:   self.name = "x"
来源：http://pym.svipenyu.cn

PHP:  public string $name = "x";
来源：http://czf.tian-w.cn

JS:   this.name = "x";
来源：http://ucr.xylfe.cn

TS:   name: string = "x";
来源：http://jkg.mhx1999.top

Java: private String name;
来源：http://lkm.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ajj.ydjk.org.cn

Ruby: @name = "x"
来源：http://slx.chenzaomai.com

C#:   public string Name { get; set; } = "x";
来源：http://hnh.zhiwuduotai.top

[G04] 定义方法
来源：http://btm.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://zfe.redwolf501.top


<!-- 参考信息 -->