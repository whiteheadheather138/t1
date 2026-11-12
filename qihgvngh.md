代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://mpo.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://pye.birdmap.top

JS:   arr.join(", ")
来源：http://frn.haohaochexian.top

TS:   arr.join(", ")
来源：http://gnf.yj20258.top

Java: String.join(", ", list)
来源：http://egu.nanxinkj.top

Go:   strings.Join(strs, ", ")
来源：http://qib.tian-w.cn

Ruby: arr.join(", ")
来源：http://ont.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://ixe.shzxlz.cn

================================================================================
来源：http://dlb.fzhhl.top

E. 字符串处理
来源：http://tki.sjlbkw.cn

================================================================================
来源：http://qyd.chenjidiqi.icu

[E01] 拼接字符串
来源：http://qsx.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dnj.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hvz.aibaodan.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jws.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yza.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dbb.jyoumei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hcb.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zgq.hfpthk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://azu.tarul.cn

[E02] 重复字符串
来源：http://bai.aibaodan.cn

Py:   "ab" * 3
来源：http://zzs.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://saw.kuanghao11.cn

JS:   "ab".repeat(3)
来源：http://opq.316326.xyz

TS:   "ab".repeat(3)
来源：http://lel.birdmap.top

Java: "ab".repeat(3)
来源：http://rky.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://ppp.c1oappe.top

Ruby: "ab" * 3
来源：http://rmy.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://exu.tarul.cn

[E03] 截取子串
来源：http://woc.nwbrower.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ymm.tanke756.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cgl.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://izv.nanxuanxn.top

TS:   s.slice(1, 4)
来源：http://baq.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://ixw.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yhk.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://pys.jiagoushi.top

C#:   s.Substring(1, 3)
来源：http://whn.hnxiangtu.top

[E04] 查找子串位置
来源：http://raz.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://cav.shangyingyoupin.top

PHP:  strpos($s, "x");
来源：http://xzu.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lcn.nanxuanxn.top

TS:   s.indexOf("x")
来源：http://maa.guowangkeji.top

Java: s.indexOf("x")
来源：http://hrq.smart0.xyz

Go:   strings.Index(s, "x")
来源：http://yiu.ctjpmb.com

Ruby: s.index("x")
来源：http://yhr.fzhhl.top

C#:   s.IndexOf("x")
来源：http://tad.pycfn.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://zkc.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xkh.ywan-chungtsiang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hgz.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kif.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zrd.sysykeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dcd.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jhb.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vau.daria6918.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oxl.yj202588.top

[E06] 替换子串
来源：http://vgg.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://att.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://irm.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aiz.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://pyp.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dil.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zrb.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lxz.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://mfk.yuxming.cn

[E07] 按分隔符拆分
来源：http://fjl.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yas.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jbs.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nyk.yj20258888.top

TS:   s.split(",")
来源：http://vti.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://bfi.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gkb.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://jpb.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oqq.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://vrv.birdmap.top

Py:   ",".join(items)
来源：http://htw.ivvv.top

PHP:  implode(",", $items);
来源：http://vxi.hysaishi.cn

JS:   items.join(",")
来源：http://pkv.316326.xyz

TS:   items.join(",")
来源：http://hex.guowangkeji.top

Java: String.join(",", items)
来源：http://fey.ivvv.top

Go:   strings.Join(items, ",")
来源：http://kwe.shangyingyoupin.top

Ruby: items.join(",")
来源：http://egb.tanke756.top

C#:   string.Join(",", items)
来源：http://mkh.smart0.xyz

[E09] 去除所有空白字符
来源：http://fvv.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://njg.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gaw.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://unw.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://vrg.fktsv.cn

Java: s.replaceAll("\\s+", "")
来源：http://ghs.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tnw.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qzq.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kjk.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://kpc.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://geu.yuanzhike.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jei.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://imw.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://lsz.ydzc1.top

Java: String.format("%03d", 7)
来源：http://rsk.bbcook.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xhu.pycfn.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wwc.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://byp.bjfxy.top

[E11] 反转字符串
来源：http://abd.sjlbkw.cn

Py:   s[::-1]
来源：http://hqv.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://mwr.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://wji.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://rks.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jyo.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fmn.fktsv.cn

Ruby: s.reverse
来源：http://yhp.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://dyf.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://xmh.52xcode.cn

Py:   s.count("a")
来源：http://eqm.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://bhy.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://wdv.sysykeji.top

TS:   s.split("a").length - 1
来源：http://vpk.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gvl.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://avn.andypj.xyz

Ruby: s.count("a")
来源：http://jcz.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://omz.daria6918.cn

[E13] 逐字符遍历
来源：http://bhz.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://ljc.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xhv.guowangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hnc.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bft.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gye.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ofw.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cnu.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qwn.nanxuanxn.top

[E14] URL 编码与 Base64
来源：http://dmz.daxiang520.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fvh.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://dnn.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jfi.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://twi.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pzi.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eff.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mym.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ewg.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://kei.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://czq.zhaomingkeji.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://olg.zhiwuduotai.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ano.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ata.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rua.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uel.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://teu.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hfa.aizwys.cn

[E16] 数字千分位
来源：http://myq.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://sqg.hesvh.cn

PHP:  number_format(1234567);
来源：http://khk.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://eky.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ogv.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jkw.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ufn.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://knu.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://msp.andypj.xyz

[E17] 首字母大写
来源：http://xgq.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mdl.ydzc1.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vug.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ukr.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tsn.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nli.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fcf.uphjek.com

Ruby: s.capitalize
来源：http://gxq.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rdv.ppjwa.cn

[E18] 模板占位符替换
来源：http://cxd.gzhubu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fik.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lgz.zhiwuduotai.top

JS:   tpl.replaceAll("{name}", name)
来源：http://usr.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xhz.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oid.nanxuanxn.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qaa.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vpk.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wgh.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://xnb.shuidangran.top

Py:   s.splitlines()
来源：http://gsl.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jlc.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://acc.gzhubu.top

TS:   s.split(/\r?\n/)
来源：http://ztv.aibaodan.cn

Java: s.lines().toList()
来源：http://qzz.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://gij.aizwys.cn

Ruby: s.lines
来源：http://ysg.gaohongyu789.top

C#:   s.Split('\n')
来源：http://lip.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://kpe.zhaomingkeji.xyz

Py:   if not s:
来源：http://blx.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ymb.guowangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zzq.guannengcc.top

TS:   if (s === "") {}
来源：http://ztm.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://nrh.jiagoushi.top

Go:   if s == "" {}
来源：http://cil.zhengqikj.top

Ruby: if s.empty?
来源：http://lae.yj202588.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xkt.xinyue.icu

[E21] 超长截断加省略号
来源：http://ggd.hfpthk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://isx.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lec.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ykn.zhaomingkeji.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rtr.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fhq.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://byg.fanxiaobao.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ibw.ywan-chungtsiang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pep.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://kdm.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sud.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zol.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wxb.havefunace.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iru.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://are.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mmh.gzhubu.top

Ruby: s.bytesize;  s.length
来源：http://jsg.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jqq.daria6918.cn

================================================================================
来源：http://lgn.9152youxi.cn

F. 文件与目录
来源：http://cnl.wangshuangyany.cn

================================================================================
来源：http://vya.hammf.cn

[F01] 读取整个文件
来源：http://tdq.xuanzx.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uuz.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://hxd.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yit.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xma.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fqk.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uqv.ybcxt.top

Ruby: File.read("a.txt")
来源：http://syk.jinqigfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://nqg.yonumen.top

[F02] 逐行读取文件
来源：http://qxw.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cuy.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yly.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://erd.cdnleiting.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vtk.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://keb.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yxt.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tgz.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uai.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://wlt.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://woh.smart0.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://edf.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://faj.jyoumei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wbg.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vnw.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hit.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://anl.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://coq.uphjek.com

[F04] 追加写入文件
来源：http://crj.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zvh.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ler.yj20258888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hsu.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://omi.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hrk.sysykeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cbt.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lpz.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qcr.jqgufenzy.top

[F05] 判断文件或目录是否存在
来源：http://rts.zhoulong.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nji.zdbjq.cn

PHP:  file_exists("a.txt");
来源：http://qgf.jinqigufen.top

JS:   fs.existsSync("a.txt")
来源：http://udz.kuanghao11.cn

TS:   fs.existsSync("a.txt")
来源：http://grs.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aki.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iks.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://ehx.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://rfo.cdnleiting.top

[F06] 删除文件
来源：http://amr.zhengqikj.top

Py:   os.remove("a.txt")
来源：http://uul.guannengcc.top

PHP:  unlink("a.txt");
来源：http://wxe.aizwys.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oks.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://ziv.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lie.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://gmi.nwbrower.top

Ruby: File.delete("a.txt")
来源：http://but.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://bmq.yfazqb.com

[F07] 创建目录（含多级）
来源：http://zxf.cucudq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pcq.dashuyun.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://loh.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nkt.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pcu.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://acz.shangyingyoupin.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ano.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ayg.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://egq.tian-w.cn

[F08] 遍历目录
来源：http://hhk.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://vnn.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://log.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://mqn.yangfankeji.com

TS:   fs.readdirSync("dir")
来源：http://gys.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://npn.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://usv.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://twu.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://jwc.jqgufenzy.top

[F09] 获取文件大小
来源：http://kdo.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://ouw.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://tqf.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://vdu.fengsongda.top

TS:   fs.statSync("a.txt").size
来源：http://jyr.yuxming.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ypq.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xos.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://ofh.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://jgo.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://yde.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ocu.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uca.ydjk.org.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oco.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://aci.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zdi.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dmj.hongshengwenyu.top


<!-- 参考信息 -->