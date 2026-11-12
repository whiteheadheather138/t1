代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://myx.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pqe.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vts.cqqwz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pab.mhx1999.top

C#:   s.Replace("a", "b")
来源：http://sgg.hesvh.cn

[E07] 按分隔符拆分
来源：http://qln.tianlin.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pey.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pap.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://szh.ybcxt.top

TS:   s.split(",")
来源：http://aay.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://qym.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ixi.yongpay.top

Ruby: s.split(",");  s.split
来源：http://fvu.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ifg.xylfe.cn

[E08] 数组按分隔符合并
来源：http://mpw.wangshuangyany.cn

Py:   ",".join(items)
来源：http://jvu.hnqzz.top

PHP:  implode(",", $items);
来源：http://gxe.yuanzhike.top

JS:   items.join(",")
来源：http://tya.haohaochexian.top

TS:   items.join(",")
来源：http://nta.ppjwa.cn

Java: String.join(",", items)
来源：http://ukm.zhongyouzk.top

Go:   strings.Join(items, ",")
来源：http://mjq.shzxlz.cn

Ruby: items.join(",")
来源：http://kcd.hfpthk.cn

C#:   string.Join(",", items)
来源：http://obk.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://bwf.hnxiangtu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://juq.aibaodan.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://feb.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://blu.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://bdk.epnwcf.com

Java: s.replaceAll("\\s+", "")
来源：http://imh.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tth.jyoumei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qgb.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rbc.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://nsj.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iut.gaohongyu789.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://naq.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://ctw.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://ing.tanke756.top

Java: String.format("%03d", 7)
来源：http://gva.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://aio.yj20258.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nqs.zhongyouzk.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vze.yueranfly.top

[E11] 反转字符串
来源：http://bvr.guowangkeji.top

Py:   s[::-1]
来源：http://kmu.yonumen.top

PHP:  strrev($s);
来源：http://ghk.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://pzu.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://flf.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cva.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ujn.shuidangran.top

Ruby: s.reverse
来源：http://ydp.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kuw.fzhhl.top

[E12] 统计某字符出现次数
来源：http://jwb.pengpengdd.cyou

Py:   s.count("a")
来源：http://lfi.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://jko.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://zyh.ybcxt.top

TS:   s.split("a").length - 1
来源：http://yeq.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gex.ydjk.org.cn

Go:   strings.Count(s, "a")
来源：http://dee.tanke756.top

Ruby: s.count("a")
来源：http://nmy.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://hcu.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://ome.yueranfly.top

Py:   for ch in s: print(ch)
来源：http://fkb.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gjf.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ygi.yj20258.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yot.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://beu.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rsh.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fnf.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ial.wangdashe.top

[E14] URL 编码与 Base64
来源：http://mij.shangyingyoupin.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uiz.gogol.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rdg.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sti.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wbd.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zei.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://izc.pycfn.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zkm.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://icy.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://mcj.vehdjk.com

Py:   html.escape(s);  html.unescape(s)
来源：http://yue.hfpthk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wfo.fktsv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ufu.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gah.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lru.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pyy.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ldy.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ilx.jianghu66.top

[E16] 数字千分位
来源：http://xhk.nwbrower.top

Py:   f"{1234567:,}"
来源：http://xgy.jianghu66.top

PHP:  number_format(1234567);
来源：http://zyo.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kxj.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gjc.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dww.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jky.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fmj.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://ffq.sysykeji.top

[E17] 首字母大写
来源：http://ydo.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://scp.zhiwuduotai.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qnh.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qae.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://igb.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fyo.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mkp.zdbjq.cn

Ruby: s.capitalize
来源：http://grj.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cxt.guowangkeji.top

[E18] 模板占位符替换
来源：http://fic.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xdv.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qqc.sxryk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nnf.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://xep.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xim.yueranfly.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nrb.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://czw.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tfg.jianghu66.top

[E19] 多行文本按行拆分
来源：http://rit.redwolf501.top

Py:   s.splitlines()
来源：http://bmv.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jdl.zhoulong.xyz

JS:   s.split(/\r?\n/)
来源：http://tuz.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://mie.cucudq.cn

Java: s.lines().toList()
来源：http://ioe.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://smd.haohaochexian.top

Ruby: s.lines
来源：http://dbf.jqgfzy.top

C#:   s.Split('\n')
来源：http://znn.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://lfi.0kj1m.cn

Py:   if not s:
来源：http://tap.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://arf.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://giy.feifeiyinyue.top

TS:   if (s === "") {}
来源：http://mlr.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://qgq.guannengcc.top

Go:   if s == "" {}
来源：http://drx.wangshuangyany.cn

Ruby: if s.empty?
来源：http://qxr.zycfv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rwl.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://teq.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://amm.vqdsnc.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ecf.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yzd.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lgo.iojbl.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rny.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://cno.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fjo.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fdv.fktsv.cn

[E22] 字节长度与字符长度
来源：http://ank.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ght.shzxlz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sft.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qht.xuanzx.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tkz.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qet.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zta.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://wwz.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ejo.redwolf501.top

================================================================================
来源：http://wok.chenjidiqi.icu

F. 文件与目录
来源：http://lfa.hammf.cn

================================================================================
来源：http://nmu.haohaochexian.top

[F01] 读取整个文件
来源：http://zmp.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ccw.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://too.cucudq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jds.vehdjk.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kqz.ywan-chungtsiang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rsb.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://exf.vqdsnc.cn

Ruby: File.read("a.txt")
来源：http://pwq.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://bzu.nwbrower.top

[F02] 逐行读取文件
来源：http://ahm.redwolf501.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xvp.wangdashe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uyk.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oce.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sao.fktsv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rrm.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://odt.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vmr.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ddg.hesvh.cn

[F03] 写入文件（覆盖）
来源：http://cnx.tarul.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sqg.jqgufenzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rgg.jinqigufen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://azi.hnqzz.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iju.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bzw.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dtt.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://ubm.kuanghao11.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zfp.epnwcf.com

[F04] 追加写入文件
来源：http://sqi.sxryk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qcv.daria6918.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ata.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yyu.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vlc.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cda.hfpthk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vvb.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kxu.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vka.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://chb.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yyg.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://dwn.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://alq.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://wtq.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dnh.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://icz.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://jmu.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://slx.hysaishi.cn

[F06] 删除文件
来源：http://pjt.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://ryi.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://pgi.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://maa.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://npz.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vym.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://sbb.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://gsd.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://agn.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://xlz.c1oappe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sqd.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://req.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rrg.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mwm.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vnj.epnwcf.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ybf.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rrb.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vps.hnxiangtu.top

[F08] 遍历目录
来源：http://lay.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rjd.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bmx.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://rjl.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://hhs.xingfuxueyuan.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dkx.aibaodan.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rpr.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://rqd.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://ofi.bjfxy.top

[F09] 获取文件大小
来源：http://qth.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://dqr.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://qbv.zhaomingkeji.xyz

JS:   fs.statSync("a.txt").size
来源：http://ytg.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://jii.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://fog.chenlongwang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zox.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://mhd.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://uon.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ilr.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rey.yanxiufei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jgw.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hkp.wangdashe.top

TS:   path.extname("a.txt")
来源：http://hnr.hfpthk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fte.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dch.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vqk.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sqs.dianchejie.cn

[F11] 复制与移动文件
来源：http://cto.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kpw.yvedp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vya.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gdb.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iag.guowangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ubs.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vvf.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pon.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ila.jqgufenzy.top

[F12] CSV 读写
来源：http://wmj.xziqi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vyx.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iiq.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xrb.ehwqpu.com

TS:   // 同上
来源：http://ubt.sxryk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xac.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ogd.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kug.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mfr.jinghuilouyu.cn

================================================================================
来源：http://lji.smart0.xyz

G. 面向对象
来源：http://uvc.gogol.net.cn

================================================================================
来源：http://ywl.jqgufenzy.top

[G01] 定义类
来源：http://cyf.zhixingplan.top

Py:   class User: pass
来源：http://xre.ydzc1.top

PHP:  class User {}
来源：http://mbo.tarul.cn

JS:   class User {}
来源：http://xll.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://yal.fzhhl.top

Java: class User {}
来源：http://rxv.sweek.top

Go:   type User struct { Name string }
来源：http://gxs.yj20258.top

Ruby: class User; end
来源：http://pol.cashguo.top

C#:   class User {}
来源：http://dnh.ywan-chungtsiang.top

[G02] 构造函数
来源：http://pqd.gzhubu.top

Py:   def __init__(self, name): self.name = name
来源：http://mul.guowangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://vgc.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://unv.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://kax.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://bzi.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jbk.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://kaf.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://gln.kuanghao11.cn

[G03] 实例属性
来源：http://pla.sufxvd.cn

Py:   self.name = "x"
来源：http://wjg.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://rus.yangfankeji.com

JS:   this.name = "x";
来源：http://xpf.jinqigfzy.top

TS:   name: string = "x";
来源：http://ang.ybcxt.top

Java: private String name;
来源：http://vcy.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ghd.ppjwa.cn

Ruby: @name = "x"
来源：http://ibr.pengpengdd.cyou

C#:   public string Name { get; set; } = "x";
来源：http://bvj.nanxuanxn.top

[G04] 定义方法
来源：http://ent.andypj.xyz

Py:   def greet(self): return self.name
来源：http://qba.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fxo.redwolf501.top

JS:   greet() { return this.name; }
来源：http://uwm.zhaomingkeji.xyz

TS:   greet(): string { return this.name; }
来源：http://qbg.chenzaomai.com

Java: String greet() { return name; }
来源：http://pau.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fib.bjfxy.top

Ruby: def greet; @name; end
来源：http://fct.yj20258.top

C#:   public string Greet() => Name;
来源：http://xdg.uphjek.com

[G05] 继承
来源：http://fzb.yvedp.cn


<!-- 参考信息 -->