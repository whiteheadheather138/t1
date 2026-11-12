代发 wailian999

PHP:  strpos($s, "x");
来源：http://jks.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://thi.sweek.top

TS:   s.indexOf("x")
来源：http://wbo.dianchejie.cn

Java: s.indexOf("x")
来源：http://kou.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://zsx.ybcxt.top

Ruby: s.index("x")
来源：http://mcq.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://lxe.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://prz.svipenyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://naz.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rbs.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ygz.yueranfly.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qjj.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://roj.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mmp.ydjk.org.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ljh.hfpthk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tic.yangfankeji.com

[E06] 替换子串
来源：http://sqs.ydzc1.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zve.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://lbi.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nmh.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://fnr.meibo888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://enj.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hen.zhaomingkeji.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mln.hammf.cn

C#:   s.Replace("a", "b")
来源：http://oqb.chenzaomai.com

[E07] 按分隔符拆分
来源：http://tyw.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kyd.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://whj.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dxv.guowangkeji.top

TS:   s.split(",")
来源：http://zmh.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rla.chenlongwang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://svb.yj202588.top

Ruby: s.split(",");  s.split
来源：http://vrh.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ksr.jinqigufen.top

[E08] 数组按分隔符合并
来源：http://jqm.pycfn.com

Py:   ",".join(items)
来源：http://wfr.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://ocx.fzhhl.top

JS:   items.join(",")
来源：http://hok.kuanghao11.cn

TS:   items.join(",")
来源：http://ikv.jlsjyb.cn

Java: String.join(",", items)
来源：http://xob.fehbvm.com

Go:   strings.Join(items, ",")
来源：http://kah.shuidangran.top

Ruby: items.join(",")
来源：http://mtz.fktsv.cn

C#:   string.Join(",", items)
来源：http://rmt.fehbvm.com

[E09] 去除所有空白字符
来源：http://wxc.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nbk.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ujm.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://wow.gogol.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://ltk.pengpengdd.cyou

Java: s.replaceAll("\\s+", "")
来源：http://mkx.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gtv.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://nbj.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fog.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://yzp.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yfr.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ysx.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://gnm.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://ebo.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://znm.yanxiufei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pyo.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ppo.cashguo.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ein.yueranfly.top

[E11] 反转字符串
来源：http://lsv.zhoulong.xyz

Py:   s[::-1]
来源：http://ptl.xuanzx.com

PHP:  strrev($s);
来源：http://mhy.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://shd.52xcode.cn

TS:   [...s].reverse().join("")
来源：http://bqa.zhiwuduotai.top

Java: new StringBuilder(s).reverse().toString()
来源：http://oxn.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jex.hysaishi.cn

Ruby: s.reverse
来源：http://dfh.ydzc1.top

C#:   new string(s.Reverse().ToArray())
来源：http://rmp.hfpthk.cn

[E12] 统计某字符出现次数
来源：http://awz.svipenyu.cn

Py:   s.count("a")
来源：http://rau.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://pye.havefunace.top

JS:   s.split("a").length - 1
来源：http://huq.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://mty.andypj.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xiw.yuxming.cn

Go:   strings.Count(s, "a")
来源：http://psr.yj20258888.top

Ruby: s.count("a")
来源：http://goi.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://nuv.aibaodan.cn

[E13] 逐字符遍历
来源：http://kow.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://ucf.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yfv.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://iyn.andypj.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://hsj.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qkq.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://msn.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://afi.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://off.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://moz.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vvy.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hwk.sysykeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lqe.shzxlz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rau.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://owa.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ase.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ntp.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cvu.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://vgl.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yhc.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hzu.zhoulong.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wqs.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iot.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hbj.316326.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aur.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xun.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gbx.zhoulong.xyz

[E16] 数字千分位
来源：http://kuj.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://arx.ybcxt.top

PHP:  number_format(1234567);
来源：http://wdn.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://maa.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://nqs.uphjek.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://deq.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vtu.jinqigufen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vpi.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://fft.guannengcc.top

[E17] 首字母大写
来源：http://gma.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vle.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nap.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zjb.andypj.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vcs.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jon.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xxa.uphjek.com

Ruby: s.capitalize
来源：http://tde.sufxvd.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wrp.yj20258.top

[E18] 模板占位符替换
来源：http://oez.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sdj.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tvu.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vyr.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rlg.yj20258.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rvm.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kyz.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kzh.yj20258888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cws.bbcook.cn

[E19] 多行文本按行拆分
来源：http://muk.nanxuanxn.top

Py:   s.splitlines()
来源：http://tih.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rrm.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://yng.ydjk.org.cn

TS:   s.split(/\r?\n/)
来源：http://yxe.ehwqpu.com

Java: s.lines().toList()
来源：http://fzd.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://urh.yongpay.top

Ruby: s.lines
来源：http://gqb.ppjwa.cn

C#:   s.Split('\n')
来源：http://xla.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://uie.vehdjk.com

Py:   if not s:
来源：http://bcn.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hfw.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pyg.aizwys.cn

TS:   if (s === "") {}
来源：http://ymu.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://ssy.yanxiufei.cn

Go:   if s == "" {}
来源：http://ldv.meibo888.top

Ruby: if s.empty?
来源：http://tqa.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kjk.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://dxm.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://obm.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xsu.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://obq.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://udu.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ozm.yanxiufei.cn

Go:   // 按 rune 判断长度后截断
来源：http://vaq.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rbh.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baa.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://aoy.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iwh.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://myc.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nww.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eoq.aizwys.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ahx.meibo888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uki.svipenyu.cn

Ruby: s.bytesize;  s.length
来源：http://kyg.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://frp.fanxiaobao.xyz

================================================================================
来源：http://wtb.xingfuxueyuan.xyz

F. 文件与目录
来源：http://ppt.xuetiantiany.cn

================================================================================
来源：http://piw.sysykeji.top

[F01] 读取整个文件
来源：http://kmh.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wpt.jinqigufen.top

PHP:  file_get_contents("a.txt");
来源：http://dje.zycfv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gcf.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sfq.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://otg.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qfu.birdmap.top

Ruby: File.read("a.txt")
来源：http://cbj.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://ocl.c1oappe.top

[F02] 逐行读取文件
来源：http://etu.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kxy.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pls.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://foz.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sca.uphjek.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zse.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dxt.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sww.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yjp.ivvv.top

[F03] 写入文件（覆盖）
来源：http://vrk.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ife.bbcook.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://aor.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hck.yanxiufei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zwv.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cmz.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hnj.fzhhl.top

Ruby: File.write("a.txt", "hi")
来源：http://yru.jyoumei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gqh.zdbjq.cn

[F04] 追加写入文件
来源：http://ghw.jqgfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hih.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://egb.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://frm.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qhr.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ehu.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ime.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xxl.aizwys.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pnz.aizwys.cn

[F05] 判断文件或目录是否存在
来源：http://cya.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wez.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://fed.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://ycv.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://oyx.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://aag.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bqd.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://nud.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://tzv.fengsongda.top

[F06] 删除文件
来源：http://cpz.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://vgl.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://awi.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://kwi.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://czf.hywenlv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xim.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://npj.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://xwn.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://qmk.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://axt.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wnr.hammf.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bzi.wangshuangyany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dqd.tian-w.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oad.aizwys.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fkc.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hnf.wangdashe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ekw.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uzw.hnxiangtu.top

[F08] 遍历目录
来源：http://kkb.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tmo.nanxinkj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yoz.sysykeji.top

JS:   fs.readdirSync("dir")
来源：http://swt.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://ogg.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jls.hnqzz.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gkh.sysykeji.top

Ruby: Dir.children("dir")
来源：http://tbe.nanxinkj.top

C#:   Directory.GetFiles("dir")
来源：http://sok.ybcxt.top

[F09] 获取文件大小
来源：http://ocr.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://wqw.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://sfd.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://bzm.zhongyouzk.top

TS:   fs.statSync("a.txt").size
来源：http://zge.epnwcf.com

Java: Files.size(Path.of("a.txt"))
来源：http://bvr.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rji.316326.xyz

Ruby: File.size("a.txt")
来源：http://jrf.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://naw.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://irk.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dwb.jlsjyb.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zur.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bhn.yvedp.cn

TS:   path.extname("a.txt")
来源：http://qbz.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bow.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gof.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rxa.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oan.tianlin.xyz

[F11] 复制与移动文件
来源：http://llw.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nne.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nml.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xmh.hywenlv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bnr.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xvg.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fhl.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fem.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jha.52xcode.cn

[F12] CSV 读写
来源：http://ris.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vao.zhongyouzk.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://htj.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://stl.jyoumei.cn

TS:   // 同上
来源：http://xlk.jqgufenzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fzv.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ssx.zhoulong.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yof.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://man.9152youxi.cn

================================================================================
来源：http://hqp.gotoacloud.top

G. 面向对象
来源：http://uhu.yueranfly.top

================================================================================
来源：http://kin.yj202588.top

[G01] 定义类
来源：http://ftb.cdnleiting.top

Py:   class User: pass
来源：http://dzw.chenzaomai.com

PHP:  class User {}
来源：http://txb.wangshuangyany.cn

JS:   class User {}
来源：http://xor.zhixingplan.top

TS:   class User { name: string = ""; }
来源：http://dcc.dashuyun.cn

Java: class User {}
来源：http://nia.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://wvb.sxryk.cn

Ruby: class User; end
来源：http://hcs.yanxiufei.cn

C#:   class User {}
来源：http://kca.zycfv.cn

[G02] 构造函数
来源：http://xnx.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://vcc.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://vlp.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://bnc.daxiang520.top

TS:   constructor(public name: string) {}
来源：http://tjl.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://wor.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yog.andypj.xyz

Ruby: def initialize(name); @name = name; end
来源：http://knv.shangyingyoupin.top


<!-- 参考信息 -->