代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lnv.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wpj.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zyu.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://unx.chenlongwang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kgj.ctjpmb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rii.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qgx.nanxinkj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dtf.yj202588.top

[E06] 替换子串
来源：http://ubz.zhengqikj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xur.yuxming.cn

PHP:  str_replace("a", "b", $s);
来源：http://wcc.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cxs.shangyingyoupin.top

TS:   s.replaceAll("a", "b")
来源：http://bcz.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iky.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pvk.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eex.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://tem.hcnkem.com

[E07] 按分隔符拆分
来源：http://xqa.haohaochexian.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iqq.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zsg.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://tku.sweek.top

TS:   s.split(",")
来源：http://iwe.xingfuxueyuan.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://alg.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ddy.jinghuilouyu.cn

Ruby: s.split(",");  s.split
来源：http://voj.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dss.cheryme.top

[E08] 数组按分隔符合并
来源：http://ppr.tianlin.xyz

Py:   ",".join(items)
来源：http://wvk.nanxuanxn.top

PHP:  implode(",", $items);
来源：http://evl.snrcjt.cn

JS:   items.join(",")
来源：http://zbu.tianlin.xyz

TS:   items.join(",")
来源：http://ptj.jyoumei.cn

Java: String.join(",", items)
来源：http://iyw.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://blf.jyoumei.cn

Ruby: items.join(",")
来源：http://jih.ctjpmb.com

C#:   string.Join(",", items)
来源：http://nyz.sweek.top

[E09] 去除所有空白字符
来源：http://mkw.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ytg.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zst.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://uvw.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://dsb.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://hde.zdbjq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kkx.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pwr.dashuyun.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dxh.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://gcq.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ctk.uphjek.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iqm.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://vje.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://kjz.wangdashe.top

Java: String.format("%03d", 7)
来源：http://kls.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lji.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uwd.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ayr.jinghuilouyu.cn

[E11] 反转字符串
来源：http://fjl.yfazqb.com

Py:   s[::-1]
来源：http://bcs.tianlin.xyz

PHP:  strrev($s);
来源：http://txk.svipenyu.cn

JS:   [...s].reverse().join("")
来源：http://ycg.meibo888.top

TS:   [...s].reverse().join("")
来源：http://swf.zhongyouzk.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qjr.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yjq.wangdashe.top

Ruby: s.reverse
来源：http://vfu.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://hjc.zhixingplan.top

[E12] 统计某字符出现次数
来源：http://bjz.zhixingplan.top

Py:   s.count("a")
来源：http://cqp.redwolf501.top

PHP:  substr_count($s, "a");
来源：http://whm.tanke756.top

JS:   s.split("a").length - 1
来源：http://xop.guannengcc.top

TS:   s.split("a").length - 1
来源：http://rgs.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gsd.hammf.cn

Go:   strings.Count(s, "a")
来源：http://foq.aizwys.cn

Ruby: s.count("a")
来源：http://hge.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://mpv.daxiang520.top

[E13] 逐字符遍历
来源：http://ltr.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://syl.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jkp.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ydw.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lla.kuanghao11.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ugv.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zxu.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kkl.jinghuilouyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uaz.ydzc1.top

[E14] URL 编码与 Base64
来源：http://dkm.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qpz.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rth.sysykeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ult.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hfg.snrcjt.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qdv.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dpo.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lpd.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yeg.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://wxf.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fgv.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tiz.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jon.yj20258888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://byo.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qwl.ivvv.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://luj.hongshengwenyu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vqc.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fje.jinqigfzy.top

[E16] 数字千分位
来源：http://ebc.andypj.xyz

Py:   f"{1234567:,}"
来源：http://bpk.yvedp.cn

PHP:  number_format(1234567);
来源：http://yjp.haohaochexian.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fyo.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ipw.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gnw.zhiwuduotai.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jzi.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tdp.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://kij.svipenyu.cn

[E17] 首字母大写
来源：http://cge.sxryk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vji.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ylp.hnqzz.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bvv.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fkq.mhx1999.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zfu.nwbrower.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dng.sufxvd.cn

Ruby: s.capitalize
来源：http://hjc.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eco.smart0.xyz

[E18] 模板占位符替换
来源：http://inz.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yft.yfazqb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fes.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iuj.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://psh.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cbu.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jny.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://drt.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://peh.hongshengwenyu.top

[E19] 多行文本按行拆分
来源：http://rmu.birdmap.top

Py:   s.splitlines()
来源：http://ijb.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xhh.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://hhg.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://rcl.sxryk.cn

Java: s.lines().toList()
来源：http://esl.wangdashe.top

Go:   strings.Split(s, "\n")
来源：http://zap.jiagoushi.top

Ruby: s.lines
来源：http://giy.9152youxi.cn

C#:   s.Split('\n')
来源：http://wwx.316326.xyz

[E20] 判断字符串是否为空
来源：http://tps.shanyushiyangkeji.top

Py:   if not s:
来源：http://pav.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://acu.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ase.gaohongyu789.top

TS:   if (s === "") {}
来源：http://qcp.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://fap.yongpay.top

Go:   if s == "" {}
来源：http://ghj.kuanghao11.cn

Ruby: if s.empty?
来源：http://uys.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iyg.smart0.xyz

[E21] 超长截断加省略号
来源：http://dcl.fktsv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gze.wangdashe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wbp.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bvb.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dgx.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://znn.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://nbe.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bmb.hysaishi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hlw.aizwys.cn

[E22] 字节长度与字符长度
来源：http://uwu.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ndp.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ugy.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iee.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dcp.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://utq.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ltj.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://kqk.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zwh.shanyushiyangkeji.top

================================================================================
来源：http://dlp.sysykeji.top

F. 文件与目录
来源：http://qwl.shanyushiyangtech.top

================================================================================
来源：http://yek.ivvv.top

[F01] 读取整个文件
来源：http://nuy.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rlb.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://yml.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nga.birdmap.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bzj.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mzq.snrcjt.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bms.yj20258888.top

Ruby: File.read("a.txt")
来源：http://ltp.hcnkem.com

C#:   File.ReadAllText("a.txt");
来源：http://fqu.guannengcc.top

[F02] 逐行读取文件
来源：http://anq.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vax.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uiy.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ncs.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uea.hcnkem.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dac.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zph.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hvi.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nro.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://eaa.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uvx.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wqh.wangdashe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ayw.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mbp.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pcm.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tlj.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://uwu.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sdf.chenzaomai.com

[F04] 追加写入文件
来源：http://smd.hesvh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jet.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gjc.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wyf.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hnn.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tgn.wangdashe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ijl.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dbc.pengpengdd.cyou

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ded.gzhubu.top

[F05] 判断文件或目录是否存在
来源：http://rhk.yj202588.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fml.hcnkem.com

PHP:  file_exists("a.txt");
来源：http://kop.ivvv.top

JS:   fs.existsSync("a.txt")
来源：http://baw.feifeiyinyue.top

TS:   fs.existsSync("a.txt")
来源：http://mcn.yongpay.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nrw.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://djx.ydjk.org.cn

Ruby: File.exist?("a.txt")
来源：http://nmx.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://yae.zhengqikj.top

[F06] 删除文件
来源：http://zml.andypj.xyz

Py:   os.remove("a.txt")
来源：http://bic.fktsv.cn

PHP:  unlink("a.txt");
来源：http://iiu.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jpr.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://nmd.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dsh.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://fpi.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://zid.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://lqp.daria6918.cn

[F07] 创建目录（含多级）
来源：http://snp.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fzp.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rsx.yj202588.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oqv.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xmg.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://flq.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://syz.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hhj.c1oappe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://suc.jinghuilouyu.cn

[F08] 遍历目录
来源：http://omb.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fld.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ywe.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://pdm.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://tbi.xingfuxueyuan.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pig.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://avv.tarul.cn

Ruby: Dir.children("dir")
来源：http://xgd.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://kpe.jinghuilouyu.cn

[F09] 获取文件大小
来源：http://sag.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://bay.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://fnz.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://rtr.fengsongda.top

TS:   fs.statSync("a.txt").size
来源：http://jya.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://tbo.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wkq.fzhhl.top

Ruby: File.size("a.txt")
来源：http://hyq.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://bqi.tarul.cn

[F10] 取文件扩展名 / 文件名
来源：http://bad.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qde.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fwj.zhijiandao.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xuw.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://bnv.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tyu.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://obh.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wfp.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ynp.zhoulong.xyz

[F11] 复制与移动文件
来源：http://ooc.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ruo.chenlongwang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mon.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://end.jinghuilouyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://boj.kuanghao11.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://epr.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gfj.hfpthk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ptr.jianghu66.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://svn.yuxming.cn

[F12] CSV 读写
来源：http://nbc.aizwys.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://htg.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dbu.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://smn.shzxlz.cn

TS:   // 同上
来源：http://wdo.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://opf.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iyz.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kld.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hok.yongpay.top

================================================================================
来源：http://ydo.jinqigfzy.top

G. 面向对象
来源：http://hcc.hnxiangtu.top

================================================================================
来源：http://dyy.jinqigfzy.top

[G01] 定义类
来源：http://jko.xuanzx.com

Py:   class User: pass
来源：http://dre.shanyushiyangtech.top

PHP:  class User {}
来源：http://blz.xziqi.cn

JS:   class User {}
来源：http://ntj.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://hyz.yuanzhike.top

Java: class User {}
来源：http://fng.ivvv.top

Go:   type User struct { Name string }
来源：http://rpl.0kj1m.cn

Ruby: class User; end
来源：http://xtb.gzhubu.top

C#:   class User {}
来源：http://vcb.9152youxi.cn

[G02] 构造函数
来源：http://kxd.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://hwu.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://yuj.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://fbn.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://kgz.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://pgu.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kqa.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://wqp.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://lyy.chenzaomai.com

[G03] 实例属性
来源：http://yxj.hnxiangtu.top

Py:   self.name = "x"
来源：http://qdx.hcnkem.com

PHP:  public string $name = "x";
来源：http://bpq.yuxming.cn

JS:   this.name = "x";
来源：http://jbl.fehbvm.com

TS:   name: string = "x";
来源：http://bmn.9152youxi.cn

Java: private String name;
来源：http://wkq.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ueb.jinqigfzy.top


<!-- 参考信息 -->