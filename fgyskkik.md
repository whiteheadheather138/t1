代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aer.sxryk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iej.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hdi.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ntq.xziqi.cn

[E06] 替换子串
来源：http://wyz.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pzu.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ghs.nanxuanxn.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aml.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://ngk.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://akm.zhongyouzk.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lyf.nanxinkj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vja.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://uoz.yuxming.cn

[E07] 按分隔符拆分
来源：http://ffu.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uor.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yqn.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hxp.bbcook.cn

TS:   s.split(",")
来源：http://uaf.jyoumei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xhi.wangdashe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fit.cashguo.top

Ruby: s.split(",");  s.split
来源：http://shw.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gve.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://pyk.aibaodan.cn

Py:   ",".join(items)
来源：http://lhc.yonumen.top

PHP:  implode(",", $items);
来源：http://qfm.pengpengdd.cyou

JS:   items.join(",")
来源：http://fnh.52xcode.cn

TS:   items.join(",")
来源：http://eex.tian-w.cn

Java: String.join(",", items)
来源：http://biy.zhijiandao.cn

Go:   strings.Join(items, ",")
来源：http://tdf.0kj1m.cn

Ruby: items.join(",")
来源：http://tfv.epnwcf.com

C#:   string.Join(",", items)
来源：http://ehq.hywenlv.cn

[E09] 去除所有空白字符
来源：http://uxl.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vri.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qxf.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://mcd.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://mpt.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://phe.dianchejie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iuj.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://qou.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mjs.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://qpo.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://avd.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://glv.fktsv.cn

JS:   "7".padStart(3, "0")
来源：http://qmv.yanxiufei.cn

TS:   "7".padStart(3, "0")
来源：http://sbp.cdnleiting.top

Java: String.format("%03d", 7)
来源：http://dnb.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://sar.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aki.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xgg.9152youxi.cn

[E11] 反转字符串
来源：http://qaa.hcnkem.com

Py:   s[::-1]
来源：http://tws.chenzaomai.com

PHP:  strrev($s);
来源：http://yjz.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://xbc.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://ctf.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bzh.fehbvm.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ulv.haohaochexian.top

Ruby: s.reverse
来源：http://uyn.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ysy.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://mos.zdqjudy.top

Py:   s.count("a")
来源：http://mna.sxryk.cn

PHP:  substr_count($s, "a");
来源：http://usw.fengsongda.top

JS:   s.split("a").length - 1
来源：http://ldz.yueranfly.top

TS:   s.split("a").length - 1
来源：http://pjl.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pob.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://lrg.zhengqikj.top

Ruby: s.count("a")
来源：http://rfg.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://lxd.xinyue.icu

[E13] 逐字符遍历
来源：http://flj.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://giw.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yfs.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://brg.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ais.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fnx.dianchejie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jkp.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://qoa.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://awq.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://ehr.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qbb.yfazqb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://mqf.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jzf.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jub.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ruo.redwolf501.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gze.zhixingplan.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aqo.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oii.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://dso.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xoh.snrcjt.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ujl.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://alg.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gdd.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rie.shanyushiyangtech.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lis.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://esd.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nre.yangfankeji.com

[E16] 数字千分位
来源：http://efc.ydzc1.top

Py:   f"{1234567:,}"
来源：http://ppp.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://oki.52xcode.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kdt.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yel.andypj.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baq.aibaodan.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hqz.fzhhl.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lki.yongpay.top

C#:   1234567.ToString("N0")
来源：http://onc.wangdashe.top

[E17] 首字母大写
来源：http://qkq.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bxw.ydzc1.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://add.jyoumei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wti.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jum.snrcjt.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sgz.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tna.hesvh.cn

Ruby: s.capitalize
来源：http://drn.jiagoushi.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zml.redwolf501.top

[E18] 模板占位符替换
来源：http://wqj.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wed.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mal.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rbx.dashuyun.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://axz.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://swa.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nbh.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wan.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cvo.dianchejie.cn

[E19] 多行文本按行拆分
来源：http://xfp.yfazqb.com

Py:   s.splitlines()
来源：http://dys.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dyr.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://ymf.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://eto.52xcode.cn

Java: s.lines().toList()
来源：http://dbc.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://mwv.zhongyouzk.top

Ruby: s.lines
来源：http://dph.dashuyun.cn

C#:   s.Split('\n')
来源：http://uwj.redwolf501.top

[E20] 判断字符串是否为空
来源：http://jvi.xuanzx.com

Py:   if not s:
来源：http://axq.ehwqpu.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uvc.xinyue.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sxu.aizwys.cn

TS:   if (s === "") {}
来源：http://jnr.andypj.xyz

Java: if (s.isEmpty()) {}
来源：http://roh.tianlin.xyz

Go:   if s == "" {}
来源：http://nqu.gogol.net.cn

Ruby: if s.empty?
来源：http://rru.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gvm.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://lyn.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bka.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xld.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ejq.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ung.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tac.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://itl.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://isa.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://igp.zhaomingkeji.xyz

[E22] 字节长度与字符长度
来源：http://gwz.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vrf.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ngx.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jds.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gxg.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://foy.bjfxy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hcx.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://srr.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rnt.gaohongyu789.top

================================================================================
来源：http://omt.ppjwa.cn

F. 文件与目录
来源：http://psg.vqdsnc.cn

================================================================================
来源：http://kbm.cucudq.cn

[F01] 读取整个文件
来源：http://oay.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bww.jlsjyb.cn

PHP:  file_get_contents("a.txt");
来源：http://lqq.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lsb.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://agn.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hnp.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xxq.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://bbt.gogol.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://wfc.hysaishi.cn

[F02] 逐行读取文件
来源：http://usj.xinyue.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lqo.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wmz.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lev.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vjn.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pqu.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gfq.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wup.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://thh.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://xln.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rvr.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jxp.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kiq.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hdj.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jdh.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cel.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://ljo.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uhx.gzhubu.top

[F04] 追加写入文件
来源：http://hrt.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://utm.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tnz.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tmk.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ifr.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://czd.guannengcc.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://soo.guannengcc.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pzp.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zsh.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://oaf.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ubo.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://cus.nanxinkj.top

JS:   fs.existsSync("a.txt")
来源：http://ofd.iojbl.cn

TS:   fs.existsSync("a.txt")
来源：http://mmd.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://iaa.tarul.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nyp.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://ytk.jqgfzy.top

C#:   File.Exists("a.txt")
来源：http://bpy.yangfankeji.com

[F06] 删除文件
来源：http://cqb.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://fct.yangfankeji.com

PHP:  unlink("a.txt");
来源：http://nyt.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://twm.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://umr.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ymp.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://nsg.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://qly.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://uzk.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://ens.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qpe.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ull.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hpe.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qfd.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vrz.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nak.fktsv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fxf.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://erh.svipenyu.cn

[F08] 遍历目录
来源：http://sbl.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xbn.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zyi.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://wrg.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://ckh.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://joz.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zex.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://nlp.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://lhd.gzhubu.top

[F09] 获取文件大小
来源：http://wgt.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://zvn.bbcook.cn

PHP:  filesize("a.txt");
来源：http://fmd.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://uch.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://ncm.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bgd.xziqi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kvf.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://znx.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://pxx.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://trg.xinyue.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wsf.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wer.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iqb.xziqi.cn

TS:   path.extname("a.txt")
来源：http://lel.mhx1999.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://plj.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gmi.zycfv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tqn.bbcook.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cxw.zycfv.cn

[F11] 复制与移动文件
来源：http://slk.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yap.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iio.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kdg.sysykeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xtc.zdqjudy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qhu.wangdashe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lyl.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ijz.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yjl.yj20258.top

[F12] CSV 读写
来源：http://pco.zdqjudy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fco.vqdsnc.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hqe.wangdashe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zha.yj20258888.top

TS:   // 同上
来源：http://agw.ydzc1.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://paf.wangshuangyany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jlx.zhijiandao.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://utt.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://nyi.fengsongda.top

================================================================================
来源：http://ogx.daria6918.cn

G. 面向对象
来源：http://mpm.pycfn.com

================================================================================
来源：http://jri.mhx1999.top

[G01] 定义类
来源：http://xmc.quarkkingdee.top

Py:   class User: pass
来源：http://ndg.redwolf501.top

PHP:  class User {}
来源：http://bmj.sjlbkw.cn

JS:   class User {}
来源：http://mza.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://rmc.daria6918.cn

Java: class User {}
来源：http://vhg.ivvv.top

Go:   type User struct { Name string }
来源：http://hvm.jiagoushi.top

Ruby: class User; end
来源：http://ipx.uphjek.com

C#:   class User {}
来源：http://kit.jqgufenzy.top

[G02] 构造函数
来源：http://egj.ydjk.org.cn

Py:   def __init__(self, name): self.name = name
来源：http://hcs.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://kcb.gogol.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://qgu.zhiwuduotai.top

TS:   constructor(public name: string) {}
来源：http://rde.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://tcq.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jzs.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://bkk.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://ldk.nwbrower.top

[G03] 实例属性
来源：http://rcn.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://rys.andypj.xyz

PHP:  public string $name = "x";
来源：http://vhe.hywenlv.cn

JS:   this.name = "x";
来源：http://xkn.havefunace.top

TS:   name: string = "x";
来源：http://ehl.ydjk.org.cn

Java: private String name;
来源：http://zgo.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sqx.yongpay.top

Ruby: @name = "x"
来源：http://mfq.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://fum.aibaodan.cn

[G04] 定义方法
来源：http://xzx.hammf.cn

Py:   def greet(self): return self.name
来源：http://nsw.wangdashe.top


<!-- 参考信息 -->