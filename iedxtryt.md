代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eqe.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wtl.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lae.ehwqpu.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ecr.shzxlz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bhi.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nav.birdmap.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fps.haohaochexian.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://seg.nwbrower.top

[E02] 重复字符串
来源：http://qor.dashuyun.cn

Py:   "ab" * 3
来源：http://yjx.cheryme.top

PHP:  str_repeat("ab", 3);
来源：http://cnm.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://urn.yuxming.cn

TS:   "ab".repeat(3)
来源：http://npf.hysaishi.cn

Java: "ab".repeat(3)
来源：http://jfy.yongpay.top

Go:   strings.Repeat("ab", 3)
来源：http://qai.shzxlz.cn

Ruby: "ab" * 3
来源：http://nib.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hcn.xuetiantiany.cn

[E03] 截取子串
来源：http://gxc.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kdu.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://csd.tarul.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kvh.fehbvm.com

TS:   s.slice(1, 4)
来源：http://uuy.chenlongwang.top

Java: s.substring(1, 4)
来源：http://lgc.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bvg.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://sik.chenlongwang.top

C#:   s.Substring(1, 3)
来源：http://qdq.yfazqb.com

[E04] 查找子串位置
来源：http://jzx.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://ahd.tarul.cn

PHP:  strpos($s, "x");
来源：http://xnv.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jct.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://gfq.ydzc1.top

Java: s.indexOf("x")
来源：http://ien.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://lbh.pengpengdd.cyou

Ruby: s.index("x")
来源：http://cwo.yj20258888.top

C#:   s.IndexOf("x")
来源：http://nio.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xjo.yueranfly.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://enj.hnxiangtu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ueu.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hew.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zkn.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sas.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fdx.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vvf.guannengcc.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zxu.zhixingplan.top

[E06] 替换子串
来源：http://ybd.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://djm.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://rfa.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xyo.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://ytc.daxiang520.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qhg.feifeiyinyue.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fcy.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jky.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://xhq.uphjek.com

[E07] 按分隔符拆分
来源：http://iht.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zft.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ijl.sjlbkw.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://esh.vqdsnc.cn

TS:   s.split(",")
来源：http://jop.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://see.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jhp.birdmap.top

Ruby: s.split(",");  s.split
来源：http://cqa.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zia.yfazqb.com

[E08] 数组按分隔符合并
来源：http://qog.cqqwz.cn

Py:   ",".join(items)
来源：http://bcs.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://ptw.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://wba.yangfankeji.com

TS:   items.join(",")
来源：http://qkz.vehdjk.com

Java: String.join(",", items)
来源：http://spg.birdmap.top

Go:   strings.Join(items, ",")
来源：http://zit.zhiwuduotai.top

Ruby: items.join(",")
来源：http://myd.bjfxy.top

C#:   string.Join(",", items)
来源：http://jua.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://tap.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fuj.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ujb.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://fto.feifeiyinyue.top

TS:   s.replace(/\s+/g, "")
来源：http://sok.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://icv.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://icg.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mju.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zfp.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://ibt.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aqr.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://frl.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://maz.guowangkeji.top

TS:   "7".padStart(3, "0")
来源：http://dba.yueranfly.top

Java: String.format("%03d", 7)
来源：http://bth.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mcs.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://amu.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pax.sjlbkw.cn

[E11] 反转字符串
来源：http://dnp.zhoulong.xyz

Py:   s[::-1]
来源：http://nxg.ehwqpu.com

PHP:  strrev($s);
来源：http://rzy.fehbvm.com

JS:   [...s].reverse().join("")
来源：http://pby.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://hgd.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wxx.nanxinkj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dnt.ydzc1.top

Ruby: s.reverse
来源：http://xol.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ljz.cheryme.top

[E12] 统计某字符出现次数
来源：http://qpf.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://pcp.jlsjyb.cn

PHP:  substr_count($s, "a");
来源：http://vys.jqgfzy.top

JS:   s.split("a").length - 1
来源：http://sou.yfazqb.com

TS:   s.split("a").length - 1
来源：http://jyy.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vfl.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://slm.nanxuanxn.top

Ruby: s.count("a")
来源：http://dja.guannengcc.top

C#:   s.Count(c => c == 'a')
来源：http://awk.yangfankeji.com

[E13] 逐字符遍历
来源：http://siz.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://yhk.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tim.zdqjudy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kig.jlsjyb.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://baq.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ddz.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ybv.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hga.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tzi.yangfankeji.com

[E14] URL 编码与 Base64
来源：http://czf.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kup.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://mse.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bmu.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uif.hnqzz.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oce.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xes.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://boi.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://smr.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://vdu.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lli.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gao.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vnt.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://han.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vef.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gra.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://egr.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kga.cdnleiting.top

[E16] 数字千分位
来源：http://apz.zycfv.cn

Py:   f"{1234567:,}"
来源：http://djr.wangdashe.top

PHP:  number_format(1234567);
来源：http://dox.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://hoo.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://udc.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://won.chenzaomai.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tra.nanxinkj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wth.guannengcc.top

C#:   1234567.ToString("N0")
来源：http://pjq.iojbl.cn

[E17] 首字母大写
来源：http://mmr.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ufd.ydzc1.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dwk.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eco.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bgm.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qsh.daria6918.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rms.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://bqd.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eeu.tarul.cn

[E18] 模板占位符替换
来源：http://uct.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cfw.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cgx.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://fgi.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ktp.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ahl.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kcp.hywenlv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://prq.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://igz.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://eil.yanxiufei.cn

Py:   s.splitlines()
来源：http://glt.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yya.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://vaz.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://tlj.bbcook.cn

Java: s.lines().toList()
来源：http://nqc.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://ybg.fengsongda.top

Ruby: s.lines
来源：http://smw.c1oappe.top

C#:   s.Split('\n')
来源：http://ona.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://kfs.yj20258888.top

Py:   if not s:
来源：http://pqx.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://psa.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nes.kuanghao11.cn

TS:   if (s === "") {}
来源：http://wxp.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://cvu.hongshengwenyu.top

Go:   if s == "" {}
来源：http://iyo.daxiang520.top

Ruby: if s.empty?
来源：http://gwp.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rdt.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://xhh.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vjt.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://plf.gzhubu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xwq.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ndm.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://elr.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://waf.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fny.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nro.cucudq.cn

[E22] 字节长度与字符长度
来源：http://esn.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://syt.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yvy.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pbc.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://itw.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xrm.zhiwuduotai.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bxm.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://pya.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://opn.hammf.cn

================================================================================
来源：http://ksz.nwbrower.top

F. 文件与目录
来源：http://hmv.0kj1m.cn

================================================================================
来源：http://bgo.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://lry.jinyuanbaomall.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zig.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://dtg.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gmx.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ttg.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sha.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mpn.vqdsnc.cn

Ruby: File.read("a.txt")
来源：http://tst.cucudq.cn

C#:   File.ReadAllText("a.txt");
来源：http://brn.bjfxy.top

[F02] 逐行读取文件
来源：http://efn.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qun.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bta.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dcq.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hwr.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jni.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cww.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://phk.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pch.yj20258.top

[F03] 写入文件（覆盖）
来源：http://vpp.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iyk.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://egb.shzxlz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hdt.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xrw.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bvd.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://civ.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://nsn.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ipe.xinyue.icu

[F04] 追加写入文件
来源：http://ize.zhongyouzk.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hua.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tln.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lhw.shangyingyoupin.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tzl.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://azs.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mmr.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tog.gzhubu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ggl.zhixingplan.top

[F05] 判断文件或目录是否存在
来源：http://obu.snrcjt.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fti.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://wsu.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://mrd.xziqi.cn

TS:   fs.existsSync("a.txt")
来源：http://jot.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uqv.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uqm.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://xwo.yj202588.top

C#:   File.Exists("a.txt")
来源：http://wwa.dianchejie.cn

[F06] 删除文件
来源：http://zsg.hfpthk.cn

Py:   os.remove("a.txt")
来源：http://itt.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://mms.yuxming.cn

JS:   fs.unlinkSync("a.txt")
来源：http://maf.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://lae.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://idb.hfpthk.cn

Go:   os.Remove("a.txt")
来源：http://umy.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://bkp.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://ifb.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://kmr.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ael.ehwqpu.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qkn.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://evq.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nng.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://taa.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://erf.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://scd.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zve.fktsv.cn

[F08] 遍历目录
来源：http://ksj.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://odj.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yhd.cheryme.top

JS:   fs.readdirSync("dir")
来源：http://dnf.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://nlq.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hnu.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hma.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://sre.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://jbr.gogol.net.cn

[F09] 获取文件大小
来源：http://hjk.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://qsk.hesvh.cn

PHP:  filesize("a.txt");
来源：http://ipr.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://wlt.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://ixv.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fqs.redwolf501.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jky.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://hnr.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://mht.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://quj.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mbd.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rjn.hesvh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ogd.cashguo.top

TS:   path.extname("a.txt")
来源：http://zpr.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fxk.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cgq.cdnleiting.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sdw.yvedp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jin.jinyuanbaomall.cn

[F11] 复制与移动文件
来源：http://kmh.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dje.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rry.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zsd.cheryme.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kbj.daria6918.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jnu.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://myz.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xfo.bbcook.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vmn.kuanghao11.cn

[F12] CSV 读写
来源：http://awk.havefunace.top


<!-- 参考信息 -->