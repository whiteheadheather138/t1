代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://jbe.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://ddy.smart0.xyz

JS:   arr.join(", ")
来源：http://bwi.52xcode.cn

TS:   arr.join(", ")
来源：http://sqe.jiagoushi.top

Java: String.join(", ", list)
来源：http://ukm.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://rdw.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://jba.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://urb.wangshuangyany.cn

================================================================================
来源：http://tnl.birdmap.top

E. 字符串处理
来源：http://qym.xinyue.icu

================================================================================
来源：http://emu.xylfe.cn

[E01] 拼接字符串
来源：http://aky.bjfxy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://msj.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ojz.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hld.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cys.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wuk.c1oappe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kel.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kqc.cdnleiting.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hch.haohaochexian.top

[E02] 重复字符串
来源：http://rac.xuanzx.com

Py:   "ab" * 3
来源：http://tva.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://mdf.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://fbn.xinyue.icu

TS:   "ab".repeat(3)
来源：http://gun.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://gtf.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://ogf.tanke756.top

Ruby: "ab" * 3
来源：http://sub.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pqx.ehwqpu.com

[E03] 截取子串
来源：http://swc.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ybu.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tdg.sysykeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dnw.ydzc1.top

TS:   s.slice(1, 4)
来源：http://gpt.aizwys.cn

Java: s.substring(1, 4)
来源：http://dxu.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cew.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://azz.xylfe.cn

C#:   s.Substring(1, 3)
来源：http://ufv.smart0.xyz

[E04] 查找子串位置
来源：http://gcl.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://icq.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://ldk.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ewv.shzxlz.cn

TS:   s.indexOf("x")
来源：http://dwz.xinyue.icu

Java: s.indexOf("x")
来源：http://ebj.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://fbd.pengpengdd.cyou

Ruby: s.index("x")
来源：http://nwj.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://csq.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zdh.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lcu.aibaodan.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mvd.ywan-chungtsiang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dmo.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pgl.birdmap.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cnl.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uwe.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ixv.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dza.chenzaomai.com

[E06] 替换子串
来源：http://bbx.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fln.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://ctb.0kj1m.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qse.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://hge.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xhr.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://crr.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hji.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://emd.sweek.top

[E07] 按分隔符拆分
来源：http://vem.yuanzhike.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kha.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tdi.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sxa.xinyue.icu

TS:   s.split(",")
来源：http://fpw.jinghuilouyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://koe.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xqv.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://mab.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gye.shanyushiyangtech.top

[E08] 数组按分隔符合并
来源：http://mcc.vqdsnc.cn

Py:   ",".join(items)
来源：http://kgo.yuanzhike.top

PHP:  implode(",", $items);
来源：http://xmd.fehbvm.com

JS:   items.join(",")
来源：http://vhl.jlsjyb.cn

TS:   items.join(",")
来源：http://urd.xylfe.cn

Java: String.join(",", items)
来源：http://nth.tanke756.top

Go:   strings.Join(items, ",")
来源：http://jbn.vqdsnc.cn

Ruby: items.join(",")
来源：http://kxm.smart0.xyz

C#:   string.Join(",", items)
来源：http://nip.ydzc1.top

[E09] 去除所有空白字符
来源：http://oph.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gfl.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ger.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://ohc.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://pzq.tianlin.xyz

Java: s.replaceAll("\\s+", "")
来源：http://cta.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://pam.chenjidiqi.icu

Ruby: s.gsub(/\s+/, "")
来源：http://ecc.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iuq.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://oxz.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ynm.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mkv.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://cmo.shanyushiyangkeji.top

TS:   "7".padStart(3, "0")
来源：http://jph.tarul.cn

Java: String.format("%03d", 7)
来源：http://zbv.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rke.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kzu.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wfw.cashguo.top

[E11] 反转字符串
来源：http://puy.nanxuanxn.top

Py:   s[::-1]
来源：http://ciw.zhixingplan.top

PHP:  strrev($s);
来源：http://vno.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://ytf.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://tiq.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xqm.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pxu.jinyuanbaomall.cn

Ruby: s.reverse
来源：http://yzv.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://yat.birdmap.top

[E12] 统计某字符出现次数
来源：http://zlh.svipenyu.cn

Py:   s.count("a")
来源：http://qtu.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://czr.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://ovb.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://awm.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wme.shanyushiyangkeji.top

Go:   strings.Count(s, "a")
来源：http://eso.tarul.cn

Ruby: s.count("a")
来源：http://xwp.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://mkw.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://aka.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://mzt.guowangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vpj.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vff.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rli.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qpy.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://daq.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://pzg.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tcr.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://jyt.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dzv.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lur.shzxlz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wnc.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ltc.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hbs.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dze.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://teh.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zud.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://mim.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://xte.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rsa.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yfo.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zww.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://alr.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hcc.0kj1m.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vvm.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://loe.hnxiangtu.top

[E16] 数字千分位
来源：http://ayp.pycfn.com

Py:   f"{1234567:,}"
来源：http://tsf.hywenlv.cn

PHP:  number_format(1234567);
来源：http://mnw.yanxiufei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ydq.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jer.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xfi.nanxinkj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fcv.yueranfly.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ayt.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://hqx.wangdashe.top

[E17] 首字母大写
来源：http://rje.kuanghao11.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oqq.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fwq.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gbb.jinqigfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fdq.pycfn.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mjg.hfpthk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ssc.xziqi.cn

Ruby: s.capitalize
来源：http://kjd.daxiang520.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ofm.shanyushiyangtech.top

[E18] 模板占位符替换
来源：http://jgk.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kdv.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tti.havefunace.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vxi.zhaomingkeji.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://rzs.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mxp.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gft.zhongyouzk.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://taq.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uqt.uphjek.com

[E19] 多行文本按行拆分
来源：http://xld.mhx1999.top

Py:   s.splitlines()
来源：http://mod.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mxk.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://sbd.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://sek.cucudq.cn

Java: s.lines().toList()
来源：http://xjm.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://pzu.redwolf501.top

Ruby: s.lines
来源：http://xbq.gzhubu.top

C#:   s.Split('\n')
来源：http://hpg.nanxinkj.top

[E20] 判断字符串是否为空
来源：http://myg.zhijiandao.cn

Py:   if not s:
来源：http://poj.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yzi.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://set.hcnkem.com

TS:   if (s === "") {}
来源：http://kdz.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://wse.ybcxt.top

Go:   if s == "" {}
来源：http://nzy.zhixingplan.top

Ruby: if s.empty?
来源：http://sxc.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://okk.jyoumei.cn

[E21] 超长截断加省略号
来源：http://enb.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ppb.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oxr.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ave.wangdashe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cgp.yueranfly.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://swq.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://ajf.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vdy.yj20258.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vmf.svipenyu.cn

[E22] 字节长度与字符长度
来源：http://tjt.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gwr.zycfv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dym.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nny.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rpq.nanxinkj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ebp.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cls.sweek.top

Ruby: s.bytesize;  s.length
来源：http://lnt.yj20258.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://upp.nanxuanxn.top

================================================================================
来源：http://ycf.316326.xyz

F. 文件与目录
来源：http://qpj.zhaomingkeji.xyz

================================================================================
来源：http://aqt.xziqi.cn

[F01] 读取整个文件
来源：http://lbu.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tch.zhongyouzk.top

PHP:  file_get_contents("a.txt");
来源：http://kpa.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://edy.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wnx.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://vfk.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vgp.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://qyf.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://bar.jianghu66.top

[F02] 逐行读取文件
来源：http://qin.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ayz.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vlf.sjlbkw.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://exl.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fsp.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://emo.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wcv.gaohongyu789.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fpl.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kmu.fktsv.cn

[F03] 写入文件（覆盖）
来源：http://njr.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uzy.yonumen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qxh.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qhb.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pxz.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kgt.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://btg.chenjidiqi.icu

Ruby: File.write("a.txt", "hi")
来源：http://sst.ydzc1.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iyl.jqgfzy.top

[F04] 追加写入文件
来源：http://pxx.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aor.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xgh.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pst.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yjk.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cey.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tow.bjfxy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bns.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hvc.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://xsa.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fiq.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://aps.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://pvz.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://vyf.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://arz.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vzv.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://feq.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://zop.jiagoushi.top

[F06] 删除文件
来源：http://fta.hongshengwenyu.top

Py:   os.remove("a.txt")
来源：http://ofu.shanyushiyangtech.top

PHP:  unlink("a.txt");
来源：http://qpu.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vja.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://wao.chenlongwang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gjj.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://iwe.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://fbs.xingfuxueyuan.xyz

C#:   File.Delete("a.txt");
来源：http://gvq.tian-w.cn

[F07] 创建目录（含多级）
来源：http://lja.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gqk.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kxk.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://csd.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ogl.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zzp.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ldp.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cvr.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dli.hywenlv.cn

[F08] 遍历目录
来源：http://ohf.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qdg.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xuh.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://rdw.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://gjg.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://igm.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jos.hammf.cn

Ruby: Dir.children("dir")
来源：http://hnn.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://ujc.jqgfzy.top

[F09] 获取文件大小
来源：http://ixp.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://hsk.iojbl.cn

PHP:  filesize("a.txt");
来源：http://zct.dianchejie.cn

JS:   fs.statSync("a.txt").size
来源：http://uij.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://hyr.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://seh.yj202588.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hue.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://yue.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://jqh.zhixingplan.top

[F10] 取文件扩展名 / 文件名
来源：http://ree.xziqi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wfz.yangfankeji.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pue.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ztr.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://gvn.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fuc.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nuh.ehwqpu.com


<!-- 参考信息 -->