代发 wailian999

Java: String.join(", ", list)
来源：http://ufd.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://ihw.wangshuangyany.cn

Ruby: arr.join(", ")
来源：http://kep.uphjek.com

C#:   string.Join(", ", list)
来源：http://vur.nanxuanxn.top

================================================================================
来源：http://tws.cucudq.cn

E. 字符串处理
来源：http://qhj.zdbjq.cn

================================================================================
来源：http://woq.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://fua.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eou.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://npx.shanyushiyangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tip.xziqi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vys.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gcp.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://seq.quarkkingdee.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cpj.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pcm.andypj.xyz

[E02] 重复字符串
来源：http://lcf.jlsjyb.cn

Py:   "ab" * 3
来源：http://ygk.andypj.xyz

PHP:  str_repeat("ab", 3);
来源：http://zun.fehbvm.com

JS:   "ab".repeat(3)
来源：http://knw.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://sga.havefunace.top

Java: "ab".repeat(3)
来源：http://dpu.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://wef.nanxuanxn.top

Ruby: "ab" * 3
来源：http://mxe.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zbt.haohaochexian.top

[E03] 截取子串
来源：http://epl.hfpthk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zxo.hongshengwenyu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gcj.fehbvm.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ovz.sysykeji.top

TS:   s.slice(1, 4)
来源：http://oob.zycfv.cn

Java: s.substring(1, 4)
来源：http://kqi.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://djj.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://hic.yvedp.cn

C#:   s.Substring(1, 3)
来源：http://pzg.gaohongyu789.top

[E04] 查找子串位置
来源：http://nff.jianghu66.top

Py:   s.find("x");  s.index("x")
来源：http://don.daxiang520.top

PHP:  strpos($s, "x");
来源：http://tvm.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://btk.redwolf501.top

TS:   s.indexOf("x")
来源：http://nbc.fktsv.cn

Java: s.indexOf("x")
来源：http://ziv.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://tpr.shangyingyoupin.top

Ruby: s.index("x")
来源：http://ntb.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://lpx.vehdjk.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://oij.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://drc.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bmc.snrcjt.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ktf.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pvx.tanke756.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cre.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ask.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wtu.fanxiaobao.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://krn.epnwcf.com

[E06] 替换子串
来源：http://ujn.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://epr.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://fes.zhiwuduotai.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jmn.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://frv.yongpay.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vjq.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lbq.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jla.cqqwz.cn

C#:   s.Replace("a", "b")
来源：http://ubq.zhixingplan.top

[E07] 按分隔符拆分
来源：http://hcu.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cgw.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jfo.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gxq.kuanghao11.cn

TS:   s.split(",")
来源：http://kcw.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://kea.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yho.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://afz.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gdz.fehbvm.com

[E08] 数组按分隔符合并
来源：http://sve.fzhhl.top

Py:   ",".join(items)
来源：http://sfy.yangfankeji.com

PHP:  implode(",", $items);
来源：http://ohj.316326.xyz

JS:   items.join(",")
来源：http://cbh.gotoacloud.top

TS:   items.join(",")
来源：http://pzt.yongpay.top

Java: String.join(",", items)
来源：http://jja.fehbvm.com

Go:   strings.Join(items, ",")
来源：http://nwx.gotoacloud.top

Ruby: items.join(",")
来源：http://tut.gotoacloud.top

C#:   string.Join(",", items)
来源：http://bst.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://ptk.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vde.fzhhl.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://unj.jqgfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://nrg.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://nem.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://onc.nanxinkj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xqc.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://pfz.shangyingyoupin.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lnt.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://jya.jinghuilouyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ghm.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bcy.nwbrower.top

JS:   "7".padStart(3, "0")
来源：http://jjk.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://dig.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://sdn.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wox.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ymj.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ujk.fktsv.cn

[E11] 反转字符串
来源：http://wqh.jqgufenzy.top

Py:   s[::-1]
来源：http://jvu.guowangkeji.top

PHP:  strrev($s);
来源：http://ngq.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://djg.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://khr.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://eex.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mux.daxiang520.top

Ruby: s.reverse
来源：http://xvi.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://txy.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://uck.shzxlz.cn

Py:   s.count("a")
来源：http://itp.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://all.jianghu66.top

JS:   s.split("a").length - 1
来源：http://cey.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://huf.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gqn.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://ipb.meibo888.top

Ruby: s.count("a")
来源：http://zol.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://qef.shzxlz.cn

[E13] 逐字符遍历
来源：http://oqi.hnqzz.top

Py:   for ch in s: print(ch)
来源：http://uzz.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ljo.pycfn.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://pso.jqgfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cdx.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cay.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bkb.iojbl.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vcm.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cwm.wangdashe.top

[E14] URL 编码与 Base64
来源：http://inf.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sya.ybcxt.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gxy.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wnv.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mgy.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://suh.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fjx.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jpf.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kif.sweek.top

[E15] HTML 转义 / 反转义
来源：http://agt.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uhi.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iij.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tmi.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lka.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bje.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tnr.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mdb.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sea.epnwcf.com

[E16] 数字千分位
来源：http://xkc.xuetiantiany.cn

Py:   f"{1234567:,}"
来源：http://rng.shuidangran.top

PHP:  number_format(1234567);
来源：http://tpx.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://unp.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zug.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zio.aizwys.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://poi.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oer.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://gnq.jyoumei.cn

[E17] 首字母大写
来源：http://ifo.sjlbkw.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hgk.hcnkem.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://fty.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vzn.shanyushiyangtech.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rkk.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nqw.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qet.wangdashe.top

Ruby: s.capitalize
来源：http://pge.jqgufenzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hfi.yanxiufei.cn

[E18] 模板占位符替换
来源：http://klv.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lxt.vqdsnc.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lwr.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://zet.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wmq.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zki.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mcg.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dfi.shanyushiyangtech.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bjl.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://dmw.ehwqpu.com

Py:   s.splitlines()
来源：http://xpm.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://snv.redwolf501.top

JS:   s.split(/\r?\n/)
来源：http://gva.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://lni.jiagoushi.top

Java: s.lines().toList()
来源：http://dye.epnwcf.com

Go:   strings.Split(s, "\n")
来源：http://ild.fehbvm.com

Ruby: s.lines
来源：http://zzx.hcnkem.com

C#:   s.Split('\n')
来源：http://qjz.snrcjt.cn

[E20] 判断字符串是否为空
来源：http://wwh.jqgufenzy.top

Py:   if not s:
来源：http://shk.xuetiantiany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fog.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fuh.yuanzhike.top

TS:   if (s === "") {}
来源：http://kjr.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://pph.daria6918.cn

Go:   if s == "" {}
来源：http://umi.pycfn.com

Ruby: if s.empty?
来源：http://ddt.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zqa.zycfv.cn

[E21] 超长截断加省略号
来源：http://bww.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rjz.xingfuxueyuan.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tcp.shanyushiyangtech.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jbg.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bgf.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zqk.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://jkh.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://muk.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mki.sufxvd.cn

[E22] 字节长度与字符长度
来源：http://knp.bbcook.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xec.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nra.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cik.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vhn.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nlg.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cnp.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://ssk.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qww.hammf.cn

================================================================================
来源：http://jpb.zhiwuduotai.top

F. 文件与目录
来源：http://csa.jinghuilouyu.cn

================================================================================
来源：http://upz.jinqigufen.top

[F01] 读取整个文件
来源：http://iip.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lla.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://rma.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ajk.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zcd.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://poj.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://age.tanke756.top

Ruby: File.read("a.txt")
来源：http://wim.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://any.fengsongda.top

[F02] 逐行读取文件
来源：http://ltg.cheryme.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iye.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dad.tianlin.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yvi.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xwk.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lsq.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dtj.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cnv.sweek.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yvt.cheryme.top

[F03] 写入文件（覆盖）
来源：http://sus.dianchejie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jvn.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rua.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eat.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vra.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://und.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eux.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://vir.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uyg.chenjidiqi.icu

[F04] 追加写入文件
来源：http://dqo.meibo888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ipi.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bzq.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cjd.ppjwa.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zdf.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wce.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dhu.ydzc1.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://atj.yongpay.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cxz.yj20258888.top

[F05] 判断文件或目录是否存在
来源：http://xfz.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ygt.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://qwf.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://fqs.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://xxo.hesvh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tmb.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://brl.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://ngf.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://pkd.hesvh.cn

[F06] 删除文件
来源：http://eyb.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://xuu.zhoulong.xyz

PHP:  unlink("a.txt");
来源：http://bmp.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://ldn.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://chc.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://agp.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://krt.hammf.cn

Ruby: File.delete("a.txt")
来源：http://yhs.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://gzy.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://nvf.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wuc.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eqe.yj202588.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cso.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ynz.yangfankeji.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://msy.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rlz.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eun.c1oappe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://faz.bjfxy.top

[F08] 遍历目录
来源：http://pvc.xuetiantiany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ukg.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hfs.hcnkem.com

JS:   fs.readdirSync("dir")
来源：http://znl.guannengcc.top

TS:   fs.readdirSync("dir")
来源：http://bho.andypj.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cxl.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ycn.sysykeji.top

Ruby: Dir.children("dir")
来源：http://amx.hywenlv.cn

C#:   Directory.GetFiles("dir")
来源：http://aab.kuanghao11.cn

[F09] 获取文件大小
来源：http://huu.zhaomingkeji.xyz

Py:   os.path.getsize("a.txt")
来源：http://exj.yonumen.top

PHP:  filesize("a.txt");
来源：http://deo.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://xsl.iojbl.cn

TS:   fs.statSync("a.txt").size
来源：http://ftm.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://ljx.xingfuxueyuan.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hlg.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://ggh.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://wjh.ppjwa.cn

[F10] 取文件扩展名 / 文件名
来源：http://nxq.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://snf.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rjj.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://azf.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://vqi.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cin.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mbh.xylfe.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gnp.gaohongyu789.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qns.shzxlz.cn

[F11] 复制与移动文件
来源：http://ruy.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sck.nwbrower.top


<!-- 参考信息 -->