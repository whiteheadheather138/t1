代发 wailian999

================================================================================
来源：http://pyl.ydzc1.top

E. 字符串处理
来源：http://vfx.c1oappe.top

================================================================================
来源：http://hws.zhaomingkeji.xyz

[E01] 拼接字符串
来源：http://fya.smart0.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lfr.jinyuanbaomall.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xmr.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gsu.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pfg.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ysy.wangshuangyany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qka.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ahx.zhoulong.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oku.cucudq.cn

[E02] 重复字符串
来源：http://oam.wangdashe.top

Py:   "ab" * 3
来源：http://ola.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://xca.bbcook.cn

JS:   "ab".repeat(3)
来源：http://dkm.yueranfly.top

TS:   "ab".repeat(3)
来源：http://ube.sufxvd.cn

Java: "ab".repeat(3)
来源：http://swj.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://ril.daria6918.cn

Ruby: "ab" * 3
来源：http://wip.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nkx.iojbl.cn

[E03] 截取子串
来源：http://rcc.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pdu.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xsa.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qvq.hysaishi.cn

TS:   s.slice(1, 4)
来源：http://guo.hysaishi.cn

Java: s.substring(1, 4)
来源：http://zks.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wjs.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://gfg.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://bol.mhx1999.top

[E04] 查找子串位置
来源：http://bvs.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://npe.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://fsj.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ttg.jqgfzy.top

TS:   s.indexOf("x")
来源：http://tqw.zhengqikj.top

Java: s.indexOf("x")
来源：http://uku.smart0.xyz

Go:   strings.Index(s, "x")
来源：http://oud.yj202588.top

Ruby: s.index("x")
来源：http://kib.wangdashe.top

C#:   s.IndexOf("x")
来源：http://ppp.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dxq.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gra.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sns.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yhb.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://sqj.c1oappe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mln.birdmap.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xpz.guannengcc.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jxu.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aae.jinqigufen.top

[E06] 替换子串
来源：http://vfd.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://crv.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://cep.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://myu.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://rfp.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fet.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fdu.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rzs.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://pbu.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://gzk.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rvy.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ggr.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://dkr.hnxiangtu.top

TS:   s.split(",")
来源：http://hzh.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://tyr.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://olb.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://und.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uvh.guannengcc.top

[E08] 数组按分隔符合并
来源：http://eus.9152youxi.cn

Py:   ",".join(items)
来源：http://yjl.cqqwz.cn

PHP:  implode(",", $items);
来源：http://fou.aizwys.cn

JS:   items.join(",")
来源：http://kkf.svipenyu.cn

TS:   items.join(",")
来源：http://bvn.hongshengwenyu.top

Java: String.join(",", items)
来源：http://ybx.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://qes.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://wfc.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://zdj.daxiang520.top

[E09] 去除所有空白字符
来源：http://ewg.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hxp.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cxt.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://dwe.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://hdh.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://rvu.chenzaomai.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://ivb.hnqzz.top

Ruby: s.gsub(/\s+/, "")
来源：http://kno.shuidangran.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://flr.sufxvd.cn

[E10] 左侧补零 / 定长填充
来源：http://kby.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://obu.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gpk.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://ete.shuidangran.top

TS:   "7".padStart(3, "0")
来源：http://ujs.tarul.cn

Java: String.format("%03d", 7)
来源：http://daz.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jpn.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cyx.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ywz.316326.xyz

[E11] 反转字符串
来源：http://mhr.yanxiufei.cn

Py:   s[::-1]
来源：http://obb.yuanzhike.top

PHP:  strrev($s);
来源：http://idb.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://euw.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://ypj.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://unh.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uiz.havefunace.top

Ruby: s.reverse
来源：http://tpj.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ffu.fengsongda.top

[E12] 统计某字符出现次数
来源：http://aku.yongpay.top

Py:   s.count("a")
来源：http://laq.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://bhg.vqdsnc.cn

JS:   s.split("a").length - 1
来源：http://mgr.yuanzhike.top

TS:   s.split("a").length - 1
来源：http://gtu.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rkk.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://arv.ydzc1.top

Ruby: s.count("a")
来源：http://ztt.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://pdk.tianlin.xyz

[E13] 逐字符遍历
来源：http://het.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://uur.andypj.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nhz.daxiang520.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gej.zhongyouzk.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hdb.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uve.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aii.ivvv.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cdk.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nhw.yj20258888.top

[E14] URL 编码与 Base64
来源：http://cyk.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bmz.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jcc.shuidangran.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ynn.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ybg.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ziw.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gbl.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://prf.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qpc.gotoacloud.top

[E15] HTML 转义 / 反转义
来源：http://moq.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dtv.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vtf.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://raa.andypj.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://shg.c1oappe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://spr.quarkkingdee.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rjd.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bjo.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jxy.fengsongda.top

[E16] 数字千分位
来源：http://qtj.jlsjyb.cn

Py:   f"{1234567:,}"
来源：http://zwp.dianchejie.cn

PHP:  number_format(1234567);
来源：http://vdb.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ptx.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://lts.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wez.chenzaomai.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oki.aizwys.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lll.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://iih.tian-w.cn

[E17] 首字母大写
来源：http://mrg.hnxiangtu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rgw.iojbl.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xih.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hxe.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wlc.yj202588.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jwn.quarkkingdee.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xqf.yueranfly.top

Ruby: s.capitalize
来源：http://uel.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ffi.shuidangran.top

[E18] 模板占位符替换
来源：http://imf.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cnf.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lgz.snrcjt.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://grd.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://had.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ufd.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qnq.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://exu.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fhm.snrcjt.cn

[E19] 多行文本按行拆分
来源：http://amg.sxryk.cn

Py:   s.splitlines()
来源：http://pwi.jinqigufen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aau.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://mxx.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://eig.yanxiufei.cn

Java: s.lines().toList()
来源：http://qiu.dashuyun.cn

Go:   strings.Split(s, "\n")
来源：http://dhx.zhoulong.xyz

Ruby: s.lines
来源：http://mgn.jianghu66.top

C#:   s.Split('\n')
来源：http://gwa.zdqjudy.top

[E20] 判断字符串是否为空
来源：http://zpv.gzhubu.top

Py:   if not s:
来源：http://dar.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://scw.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zqd.dianchejie.cn

TS:   if (s === "") {}
来源：http://scg.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://clb.mhx1999.top

Go:   if s == "" {}
来源：http://qpl.andypj.xyz

Ruby: if s.empty?
来源：http://aes.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://akx.yj20258888.top

[E21] 超长截断加省略号
来源：http://nhd.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wpo.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://drp.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://byg.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eho.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qsg.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://inf.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pko.ivvv.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xhw.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://syq.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uzt.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ftm.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cgg.shzxlz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xnv.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://crh.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kvz.gzhubu.top

Ruby: s.bytesize;  s.length
来源：http://ozl.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://agw.yonumen.top

================================================================================
来源：http://hav.meibo888.top

F. 文件与目录
来源：http://eaw.yvedp.cn

================================================================================
来源：http://amu.sxryk.cn

[F01] 读取整个文件
来源：http://nxy.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pet.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://sif.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mya.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://euw.andypj.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://ckn.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xpa.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://nws.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://wcn.birdmap.top

[F02] 逐行读取文件
来源：http://duo.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zhz.sysykeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://btu.bjfxy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hyo.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jwz.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rvd.cqqwz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bpv.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vqm.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xfd.vehdjk.com

[F03] 写入文件（覆盖）
来源：http://qtv.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cyx.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bxk.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://age.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ljn.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bmp.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://byc.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://bgw.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ynz.bjfxy.top

[F04] 追加写入文件
来源：http://aje.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jgf.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://acv.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pih.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nze.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://olp.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iuj.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yng.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://itv.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://rdf.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://idn.fktsv.cn

PHP:  file_exists("a.txt");
来源：http://cjo.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://ewd.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://omf.sjlbkw.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fvr.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xyc.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://ttl.uphjek.com

C#:   File.Exists("a.txt")
来源：http://ftn.52xcode.cn

[F06] 删除文件
来源：http://lww.vehdjk.com

Py:   os.remove("a.txt")
来源：http://jol.andypj.xyz

PHP:  unlink("a.txt");
来源：http://cfy.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://mpp.pengpengdd.cyou

TS:   fs.unlinkSync("a.txt")
来源：http://mvf.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vlq.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://ner.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://oel.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://ojf.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://fug.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vjs.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hje.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vro.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rlv.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ffz.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://usq.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ygv.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ehe.jinghuilouyu.cn

[F08] 遍历目录
来源：http://guo.zdbjq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aiy.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://axw.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://kdh.haohaochexian.top

TS:   fs.readdirSync("dir")
来源：http://xnn.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gzb.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jsg.quarkkingdee.top

Ruby: Dir.children("dir")
来源：http://oef.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://rws.cucudq.cn

[F09] 获取文件大小
来源：http://gnm.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://nhz.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://ktm.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://pzn.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://sla.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nxe.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uvj.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://qrv.shzxlz.cn

C#:   new FileInfo("a.txt").Length
来源：http://mnq.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://cwo.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wqx.shuidangran.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qex.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tiz.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://vfl.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jjp.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cut.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lre.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kgy.c1oappe.top

[F11] 复制与移动文件
来源：http://xtx.aizwys.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hef.dianchejie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dtm.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wnu.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ktx.xylfe.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qlo.sweek.top


<!-- 参考信息 -->