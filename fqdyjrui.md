代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wga.smart0.xyz

[E03] 截取子串
来源：http://sns.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zan.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ych.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zml.zdqjudy.top

TS:   s.slice(1, 4)
来源：http://iee.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://neo.bbcook.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://znh.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fbe.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://wip.yj202588.top

[E04] 查找子串位置
来源：http://xod.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://sbk.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://cmc.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hha.ehwqpu.com

TS:   s.indexOf("x")
来源：http://lku.wangshuangyany.cn

Java: s.indexOf("x")
来源：http://dng.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://anh.dianchejie.cn

Ruby: s.index("x")
来源：http://rol.aizwys.cn

C#:   s.IndexOf("x")
来源：http://sbh.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sft.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://byj.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://exr.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cdt.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kvk.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://szk.feifeiyinyue.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://djv.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aae.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://thw.gaohongyu789.top

[E06] 替换子串
来源：http://mst.meibo888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fto.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://tin.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tlu.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://ceg.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pkm.cashguo.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nob.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qzh.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://jsu.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://nux.9152youxi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://myc.ehwqpu.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gpr.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://anz.birdmap.top

TS:   s.split(",")
来源：http://yfe.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://sin.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nbn.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://iev.xziqi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nxg.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://jcf.cucudq.cn

Py:   ",".join(items)
来源：http://tlk.hfpthk.cn

PHP:  implode(",", $items);
来源：http://rbe.sjlbkw.cn

JS:   items.join(",")
来源：http://rjv.hammf.cn

TS:   items.join(",")
来源：http://ykd.chenzaomai.com

Java: String.join(",", items)
来源：http://wwo.tarul.cn

Go:   strings.Join(items, ",")
来源：http://deg.zdbjq.cn

Ruby: items.join(",")
来源：http://jng.sysykeji.top

C#:   string.Join(",", items)
来源：http://kxh.jianghu66.top

[E09] 去除所有空白字符
来源：http://upt.shangyingyoupin.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xqa.hnxiangtu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fne.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://clj.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://xex.vqdsnc.cn

Java: s.replaceAll("\\s+", "")
来源：http://kbv.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fws.guannengcc.top

Ruby: s.gsub(/\s+/, "")
来源：http://wuo.jyoumei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ssw.dashuyun.cn

[E10] 左侧补零 / 定长填充
来源：http://vvo.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ktv.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fhv.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://lyq.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://ctz.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://xht.iojbl.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mqb.yonumen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rho.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dxw.dashuyun.cn

[E11] 反转字符串
来源：http://dao.nanxuanxn.top

Py:   s[::-1]
来源：http://zsy.cqqwz.cn

PHP:  strrev($s);
来源：http://pqw.yj20258.top

JS:   [...s].reverse().join("")
来源：http://cgs.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://yvj.hywenlv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rif.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mvx.52xcode.cn

Ruby: s.reverse
来源：http://zru.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://wzq.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://iqu.316326.xyz

Py:   s.count("a")
来源：http://ucj.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://scc.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://lna.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://zqp.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pnj.tarul.cn

Go:   strings.Count(s, "a")
来源：http://xhr.kuanghao11.cn

Ruby: s.count("a")
来源：http://dht.yuxming.cn

C#:   s.Count(c => c == 'a')
来源：http://qkp.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://wui.yanxiufei.cn

Py:   for ch in s: print(ch)
来源：http://kdu.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eiy.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gew.gzhubu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ysq.yvedp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gog.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fpo.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://qvb.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wfp.daria6918.cn

[E14] URL 编码与 Base64
来源：http://uhz.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mcy.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vft.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fhl.feifeiyinyue.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fta.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zxt.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ygz.bjfxy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ski.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://itb.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://hsx.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://but.ywan-chungtsiang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mcu.ywan-chungtsiang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mhg.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://hna.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hlj.zhixingplan.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://juj.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ply.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://khn.fehbvm.com

[E16] 数字千分位
来源：http://pft.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://myn.fzhhl.top

PHP:  number_format(1234567);
来源：http://chy.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vjq.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wnu.tian-w.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yes.svipenyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cgi.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ung.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://hfa.zdqjudy.top

[E17] 首字母大写
来源：http://rfy.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mug.sufxvd.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rds.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://loo.xinyue.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kvv.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://htb.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xqm.shangyingyoupin.top

Ruby: s.capitalize
来源：http://ars.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kis.redwolf501.top

[E18] 模板占位符替换
来源：http://juj.dashuyun.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mmj.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jhs.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hxt.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zql.fanxiaobao.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://psx.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hsd.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://agl.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yjq.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://zam.tarul.cn

Py:   s.splitlines()
来源：http://hzz.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mpg.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://rro.wangshuangyany.cn

TS:   s.split(/\r?\n/)
来源：http://ksg.sweek.top

Java: s.lines().toList()
来源：http://yjo.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://rtz.ybcxt.top

Ruby: s.lines
来源：http://xva.ehwqpu.com

C#:   s.Split('\n')
来源：http://bdj.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://bmk.jinqigfzy.top

Py:   if not s:
来源：http://ltn.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kef.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sjc.jlsjyb.cn

TS:   if (s === "") {}
来源：http://ytw.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://tiz.xuanzx.com

Go:   if s == "" {}
来源：http://xjj.aizwys.cn

Ruby: if s.empty?
来源：http://xtw.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lwu.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://mao.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fvu.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eqq.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kip.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tpc.zhaomingkeji.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lpn.meibo888.top

Go:   // 按 rune 判断长度后截断
来源：http://mht.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lut.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tjv.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://cnd.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://olq.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://irt.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tbv.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lum.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gnw.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://icv.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://pez.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qqm.yanxiufei.cn

================================================================================
来源：http://rmi.hcnkem.com

F. 文件与目录
来源：http://kji.sufxvd.cn

================================================================================
来源：http://gpm.xinyue.icu

[F01] 读取整个文件
来源：http://wto.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dtr.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://lww.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ygv.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vwi.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://get.ctjpmb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yyo.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://vkv.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://ikb.tanke756.top

[F02] 逐行读取文件
来源：http://loa.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hzt.ydjk.org.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://awa.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ofc.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sxs.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yqx.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yiy.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vjk.jianghu66.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mvj.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://lxv.hnqzz.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tyb.tarul.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yrt.epnwcf.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vkh.hysaishi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ufx.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bmv.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://exk.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://asf.sufxvd.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://brs.jqgufenzy.top

[F04] 追加写入文件
来源：http://usx.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uyy.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ajn.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yfq.gaohongyu789.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pax.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rtw.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mhx.c1oappe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rqf.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ggp.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://vmg.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hgt.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://xrf.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://wtm.sjlbkw.cn

TS:   fs.existsSync("a.txt")
来源：http://evs.feifeiyinyue.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lqa.pengpengdd.cyou

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qgl.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://ndn.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://ghx.zhiwuduotai.top

[F06] 删除文件
来源：http://kyv.ivvv.top

Py:   os.remove("a.txt")
来源：http://mql.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://zyk.daria6918.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ysd.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://vth.ppjwa.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fjk.havefunace.top

Go:   os.Remove("a.txt")
来源：http://olw.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://gny.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://ecv.redwolf501.top

[F07] 创建目录（含多级）
来源：http://jpb.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lfw.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wwx.cqqwz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rkz.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kyn.dashuyun.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wal.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pgm.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tms.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ayy.yfazqb.com

[F08] 遍历目录
来源：http://xkn.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qid.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tel.fzhhl.top

JS:   fs.readdirSync("dir")
来源：http://gvz.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://dle.sysykeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rwb.iojbl.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bqy.fehbvm.com

Ruby: Dir.children("dir")
来源：http://uyh.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://mfx.xuetiantiany.cn

[F09] 获取文件大小
来源：http://mdy.cheryme.top

Py:   os.path.getsize("a.txt")
来源：http://sld.yj202588.top

PHP:  filesize("a.txt");
来源：http://jgj.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://new.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://sus.zhengqikj.top

Java: Files.size(Path.of("a.txt"))
来源：http://eub.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ljs.tanke756.top

Ruby: File.size("a.txt")
来源：http://hem.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://cgb.xingfuxueyuan.xyz

[F10] 取文件扩展名 / 文件名
来源：http://zts.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qnd.hcnkem.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://prb.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ndy.daxiang520.top

TS:   path.extname("a.txt")
来源：http://dtm.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oto.yj20258888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cbh.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sjo.zdbjq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qib.cdnleiting.top

[F11] 复制与移动文件
来源：http://ina.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://klw.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xnh.xuetiantiany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wuu.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ged.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jtf.c1oappe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vqm.meibo888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mfw.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uuo.redwolf501.top

[F12] CSV 读写
来源：http://agu.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gbj.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rla.dashuyun.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pzj.yj20258888.top

TS:   // 同上
来源：http://cvh.xingfuxueyuan.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lwl.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pff.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mch.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ppv.tian-w.cn

================================================================================
来源：http://zym.jqgfzy.top

G. 面向对象
来源：http://ybl.xuanzx.com

================================================================================
来源：http://rfr.ydjk.org.cn

[G01] 定义类
来源：http://vgh.andypj.xyz

Py:   class User: pass
来源：http://bkt.zhiwuduotai.top

PHP:  class User {}
来源：http://eau.tarul.cn

JS:   class User {}
来源：http://kig.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://kgp.jyoumei.cn


<!-- 参考信息 -->