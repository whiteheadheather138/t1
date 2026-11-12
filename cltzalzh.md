代发 wailian999

[E02] 重复字符串
来源：http://pgw.ehwqpu.com

Py:   "ab" * 3
来源：http://vde.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://sph.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://osx.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://gis.ydzc1.top

Java: "ab".repeat(3)
来源：http://rsd.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://zih.pycfn.com

Ruby: "ab" * 3
来源：http://umz.zhixingplan.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gth.tanke756.top

[E03] 截取子串
来源：http://njc.jinghuilouyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jvc.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ckp.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ehu.yfazqb.com

TS:   s.slice(1, 4)
来源：http://uaz.zhengqikj.top

Java: s.substring(1, 4)
来源：http://gnw.bbcook.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wdp.hcnkem.com

Ruby: s[1, 3];  s[1..3]
来源：http://hwo.ywan-chungtsiang.top

C#:   s.Substring(1, 3)
来源：http://ruh.xuetiantiany.cn

[E04] 查找子串位置
来源：http://nps.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://hvq.epnwcf.com

PHP:  strpos($s, "x");
来源：http://qsx.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pot.xingfuxueyuan.xyz

TS:   s.indexOf("x")
来源：http://sjy.quarkkingdee.top

Java: s.indexOf("x")
来源：http://hij.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://xov.tarul.cn

Ruby: s.index("x")
来源：http://rjh.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://kad.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vam.shuidangran.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zdf.hcnkem.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pay.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ghh.yj202588.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zhh.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://syv.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hfn.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mtp.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gzw.tian-w.cn

[E06] 替换子串
来源：http://ncg.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fzj.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://oee.uphjek.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jkf.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://bug.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qtu.cashguo.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kwa.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aje.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://vdx.fzhhl.top

[E07] 按分隔符拆分
来源：http://sfc.sufxvd.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fit.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zrf.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://exd.yj202588.top

TS:   s.split(",")
来源：http://yxu.52xcode.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pog.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xvf.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://ddv.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hhg.meibo888.top

[E08] 数组按分隔符合并
来源：http://puk.yueranfly.top

Py:   ",".join(items)
来源：http://jdy.xylfe.cn

PHP:  implode(",", $items);
来源：http://efr.fzhhl.top

JS:   items.join(",")
来源：http://wki.yonumen.top

TS:   items.join(",")
来源：http://ziu.dianchejie.cn

Java: String.join(",", items)
来源：http://dvz.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://rje.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://cqz.jianghu66.top

C#:   string.Join(",", items)
来源：http://qyf.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://xop.ppjwa.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qxc.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rla.zhongyouzk.top

JS:   s.replace(/\s+/g, "")
来源：http://ulg.zycfv.cn

TS:   s.replace(/\s+/g, "")
来源：http://npj.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://odb.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rrn.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://pcb.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sph.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://zfb.gzhubu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cba.fktsv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bad.yuanzhike.top

JS:   "7".padStart(3, "0")
来源：http://cfo.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://kpa.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://wjr.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vge.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kfo.pengpengdd.cyou

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://etk.daria6918.cn

[E11] 反转字符串
来源：http://wwp.sufxvd.cn

Py:   s[::-1]
来源：http://iur.yvedp.cn

PHP:  strrev($s);
来源：http://wma.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://car.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://mow.ybcxt.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bda.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rsn.xuanzx.com

Ruby: s.reverse
来源：http://ins.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://ilz.cqqwz.cn

[E12] 统计某字符出现次数
来源：http://arr.jlsjyb.cn

Py:   s.count("a")
来源：http://kko.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://fpf.daxiang520.top

JS:   s.split("a").length - 1
来源：http://npo.jyoumei.cn

TS:   s.split("a").length - 1
来源：http://shu.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iqr.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://mvb.9152youxi.cn

Ruby: s.count("a")
来源：http://fyw.tarul.cn

C#:   s.Count(c => c == 'a')
来源：http://ftb.pengpengdd.cyou

[E13] 逐字符遍历
来源：http://qfy.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://bvh.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xus.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://svh.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://gxq.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dlh.tarul.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://twf.epnwcf.com

Ruby: s.each_char { |ch| puts ch }
来源：http://tpn.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blm.hesvh.cn

[E14] URL 编码与 Base64
来源：http://upz.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dsj.cashguo.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rdn.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://niv.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://woe.zycfv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xax.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://drt.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://atw.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qxk.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://siu.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gmz.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fmm.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mqr.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pfs.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dno.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wxh.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tds.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mid.jinqigfzy.top

[E16] 数字千分位
来源：http://udw.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://vcu.tarul.cn

PHP:  number_format(1234567);
来源：http://vdg.gotoacloud.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hzk.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tkk.haohaochexian.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fxs.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rdy.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bhy.tarul.cn

C#:   1234567.ToString("N0")
来源：http://ntr.iojbl.cn

[E17] 首字母大写
来源：http://svk.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gnt.zhiwuduotai.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xdk.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lcs.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lzq.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pld.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://klq.yj202588.top

Ruby: s.capitalize
来源：http://mlb.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://orz.gotoacloud.top

[E18] 模板占位符替换
来源：http://kqf.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lzd.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bek.haohaochexian.top

JS:   tpl.replaceAll("{name}", name)
来源：http://avs.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://whx.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oob.chenzaomai.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wqp.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rtx.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lkf.shuidangran.top

[E19] 多行文本按行拆分
来源：http://rfl.bbcook.cn

Py:   s.splitlines()
来源：http://pzl.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ijj.nanxuanxn.top

JS:   s.split(/\r?\n/)
来源：http://jxv.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://edz.zdbjq.cn

Java: s.lines().toList()
来源：http://rja.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://mbg.shanyushiyangtech.top

Ruby: s.lines
来源：http://nba.yj20258888.top

C#:   s.Split('\n')
来源：http://zon.tanke756.top

[E20] 判断字符串是否为空
来源：http://vft.hywenlv.cn

Py:   if not s:
来源：http://fyh.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://awq.yanxiufei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pjq.xylfe.cn

TS:   if (s === "") {}
来源：http://zwq.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://vth.sxryk.cn

Go:   if s == "" {}
来源：http://aej.daria6918.cn

Ruby: if s.empty?
来源：http://sez.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://taq.fengsongda.top

[E21] 超长截断加省略号
来源：http://fev.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bvf.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nub.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kpo.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zrr.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hqj.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://cpw.bbcook.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fyh.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jot.mhx1999.top

[E22] 字节长度与字符长度
来源：http://aai.havefunace.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ayz.c1oappe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wrz.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ooq.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kev.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xmk.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rdd.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://qwd.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://but.yfazqb.com

================================================================================
来源：http://eun.zhengqikj.top

F. 文件与目录
来源：http://amb.jinghuilouyu.cn

================================================================================
来源：http://mbg.xuetiantiany.cn

[F01] 读取整个文件
来源：http://bkh.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://psy.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://lpn.sysykeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dtx.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qnu.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hbs.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iqq.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://fgf.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://gmr.yangfankeji.com

[F02] 逐行读取文件
来源：http://qbd.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lzr.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://omr.gaohongyu789.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eyy.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ofq.gotoacloud.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ukr.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wbx.jiagoushi.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://thw.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dqt.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://who.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vfm.nanxinkj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rgl.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dyk.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hou.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://znn.zhiwuduotai.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mxp.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://eff.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bws.tian-w.cn

[F04] 追加写入文件
来源：http://qqv.andypj.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vlj.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://han.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kfn.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yby.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yof.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qlx.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cyq.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ory.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://doy.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yex.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://llh.yangfankeji.com

JS:   fs.existsSync("a.txt")
来源：http://qmb.sweek.top

TS:   fs.existsSync("a.txt")
来源：http://usk.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ujp.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://puz.zhixingplan.top

Ruby: File.exist?("a.txt")
来源：http://juc.tanke756.top

C#:   File.Exists("a.txt")
来源：http://mwu.gotoacloud.top

[F06] 删除文件
来源：http://mui.bbcook.cn

Py:   os.remove("a.txt")
来源：http://qjp.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://qop.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://wvy.chenlongwang.top

TS:   fs.unlinkSync("a.txt")
来源：http://yfh.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mcs.chenjidiqi.icu

Go:   os.Remove("a.txt")
来源：http://cth.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://cgk.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://cso.316326.xyz

[F07] 创建目录（含多级）
来源：http://pji.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dem.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mbh.yj20258888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cxx.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wwk.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oni.sweek.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bqn.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://upt.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gkc.tianlin.xyz

[F08] 遍历目录
来源：http://yxz.jinqigufen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://czf.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://emv.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://brb.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://bgj.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uee.sufxvd.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://die.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://cus.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://wcp.aibaodan.cn

[F09] 获取文件大小
来源：http://rpw.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://zau.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://ojl.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://tmo.zdbjq.cn

TS:   fs.statSync("a.txt").size
来源：http://kqw.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://bfs.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kgi.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://nok.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://svj.cqqwz.cn

[F10] 取文件扩展名 / 文件名
来源：http://xjz.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mkg.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zft.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dxl.meibo888.top

TS:   path.extname("a.txt")
来源：http://kwh.yfazqb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ilq.yj202588.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://opt.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bye.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tmn.smart0.xyz

[F11] 复制与移动文件
来源：http://pye.zhoulong.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://czi.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gcw.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cgb.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://olf.jinqigfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://roi.havefunace.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yls.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bhe.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gjq.yj20258.top

[F12] CSV 读写
来源：http://luf.guowangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ssc.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iwx.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vfj.xziqi.cn

TS:   // 同上
来源：http://xnv.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wlg.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ctx.cashguo.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bop.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wdy.havefunace.top


<!-- 参考信息 -->