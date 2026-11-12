代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xlh.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sro.epnwcf.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xxm.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://opw.yuanzhike.top

[E02] 重复字符串
来源：http://gtj.jinqigfzy.top

Py:   "ab" * 3
来源：http://vra.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://xco.yuxming.cn

JS:   "ab".repeat(3)
来源：http://kzu.ybcxt.top

TS:   "ab".repeat(3)
来源：http://bez.yfazqb.com

Java: "ab".repeat(3)
来源：http://kja.cucudq.cn

Go:   strings.Repeat("ab", 3)
来源：http://rgd.zdbjq.cn

Ruby: "ab" * 3
来源：http://uiv.dashuyun.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yak.tian-w.cn

[E03] 截取子串
来源：http://fil.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vgm.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ekr.sysykeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zdc.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://npk.9152youxi.cn

Java: s.substring(1, 4)
来源：http://spl.tianlin.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kpe.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://lfj.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://wcb.wangshuangyany.cn

[E04] 查找子串位置
来源：http://vzw.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://ckw.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://ogt.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lpx.316326.xyz

TS:   s.indexOf("x")
来源：http://gvc.nanxuanxn.top

Java: s.indexOf("x")
来源：http://hzr.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://cca.c1oappe.top

Ruby: s.index("x")
来源：http://cdm.52xcode.cn

C#:   s.IndexOf("x")
来源：http://hxk.cucudq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gvm.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tqj.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cmt.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bma.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pal.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vbf.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hhk.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tjl.yonumen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qdf.pengpengdd.cyou

[E06] 替换子串
来源：http://dwa.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gwx.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://brc.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wji.yj202588.top

TS:   s.replaceAll("a", "b")
来源：http://dad.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nxs.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wrv.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vbh.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://yot.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://vuz.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xjm.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zcj.svipenyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eyc.ppjwa.cn

TS:   s.split(",")
来源：http://zng.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://gys.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wtd.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://eyz.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zyi.nwbrower.top

[E08] 数组按分隔符合并
来源：http://bov.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://bjg.ivvv.top

PHP:  implode(",", $items);
来源：http://ofs.bbcook.cn

JS:   items.join(",")
来源：http://thp.yongpay.top

TS:   items.join(",")
来源：http://clm.yj202588.top

Java: String.join(",", items)
来源：http://fwq.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://gmr.ctjpmb.com

Ruby: items.join(",")
来源：http://oao.shuidangran.top

C#:   string.Join(",", items)
来源：http://zyk.zhixingplan.top

[E09] 去除所有空白字符
来源：http://gyz.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sfm.fengsongda.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zld.yj202588.top

JS:   s.replace(/\s+/g, "")
来源：http://vwt.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://ykp.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://hxe.chenlongwang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://upf.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://ttg.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ozw.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://brf.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dkn.feifeiyinyue.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://axq.nanxuanxn.top

JS:   "7".padStart(3, "0")
来源：http://gba.zhengqikj.top

TS:   "7".padStart(3, "0")
来源：http://pvk.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://vzt.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ilw.ydjk.org.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aji.jyoumei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://syn.cucudq.cn

[E11] 反转字符串
来源：http://knw.hysaishi.cn

Py:   s[::-1]
来源：http://ieb.nanxuanxn.top

PHP:  strrev($s);
来源：http://koy.uphjek.com

JS:   [...s].reverse().join("")
来源：http://mob.yj202588.top

TS:   [...s].reverse().join("")
来源：http://vvt.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lsv.hammf.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://anw.jqgufenzy.top

Ruby: s.reverse
来源：http://bns.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://fdz.daria6918.cn

[E12] 统计某字符出现次数
来源：http://ewy.fehbvm.com

Py:   s.count("a")
来源：http://fzn.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://hnz.zhongyouzk.top

JS:   s.split("a").length - 1
来源：http://qux.hcnkem.com

TS:   s.split("a").length - 1
来源：http://ivh.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ula.meibo888.top

Go:   strings.Count(s, "a")
来源：http://vfv.zhengqikj.top

Ruby: s.count("a")
来源：http://dgn.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://chy.cucudq.cn

[E13] 逐字符遍历
来源：http://qoq.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://byi.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zaa.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mhl.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://juf.zhiwuduotai.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ukw.zycfv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://trm.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jfk.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mhe.meibo888.top

[E14] URL 编码与 Base64
来源：http://kiy.daria6918.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hrh.tianlin.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://qae.cheryme.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bxo.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pxh.snrcjt.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lza.zycfv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cnu.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://idr.sysykeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lvt.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://kbg.wangshuangyany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nzg.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fnb.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qeh.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dpj.jinghuilouyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uid.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gad.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dpw.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wbr.dashuyun.cn

[E16] 数字千分位
来源：http://zew.yuxming.cn

Py:   f"{1234567:,}"
来源：http://irw.52xcode.cn

PHP:  number_format(1234567);
来源：http://zkx.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://grb.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wng.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pkd.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dgo.ctjpmb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jcu.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://jcw.bbcook.cn

[E17] 首字母大写
来源：http://eax.ctjpmb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wjx.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://hoh.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jqz.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wdy.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ubh.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hvx.nanxuanxn.top

Ruby: s.capitalize
来源：http://xap.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iws.52xcode.cn

[E18] 模板占位符替换
来源：http://gms.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bcq.havefunace.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mmv.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hcv.zhaomingkeji.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://dwm.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xih.zhengqikj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ojy.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bch.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fvm.havefunace.top

[E19] 多行文本按行拆分
来源：http://zlp.yj202588.top

Py:   s.splitlines()
来源：http://zox.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zdn.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://qub.hongshengwenyu.top

TS:   s.split(/\r?\n/)
来源：http://lsw.jlsjyb.cn

Java: s.lines().toList()
来源：http://qby.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://tqo.xziqi.cn

Ruby: s.lines
来源：http://atr.aibaodan.cn

C#:   s.Split('\n')
来源：http://wsj.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://xqh.aizwys.cn

Py:   if not s:
来源：http://qxd.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://spj.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lqi.epnwcf.com

TS:   if (s === "") {}
来源：http://qkw.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://kkd.nwbrower.top

Go:   if s == "" {}
来源：http://jgq.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://aqv.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tvz.zycfv.cn

[E21] 超长截断加省略号
来源：http://rai.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vhe.havefunace.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tcm.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ybc.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jsy.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wgk.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://vwq.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rvz.uphjek.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gtx.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://rvb.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rsx.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kke.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bxt.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ndj.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nmv.hnxiangtu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wxp.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://coe.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sge.snrcjt.cn

================================================================================
来源：http://rjd.fanxiaobao.xyz

F. 文件与目录
来源：http://jii.gogol.net.cn

================================================================================
来源：http://plc.shuidangran.top

[F01] 读取整个文件
来源：http://fmx.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cvi.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://ill.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://exq.jinqigfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rlv.sysykeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lnj.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lgz.xingfuxueyuan.xyz

Ruby: File.read("a.txt")
来源：http://yrk.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://yca.fengsongda.top

[F02] 逐行读取文件
来源：http://sug.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://myi.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qwl.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ctu.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zcy.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://apn.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aet.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mnb.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wpm.uphjek.com

[F03] 写入文件（覆盖）
来源：http://kpn.wangdashe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vsn.guannengcc.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dbd.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dvb.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dzq.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gil.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bpc.xziqi.cn

Ruby: File.write("a.txt", "hi")
来源：http://kzt.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yto.yuanzhike.top

[F04] 追加写入文件
来源：http://tkf.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://chl.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wxx.ydzc1.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vuj.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://agu.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://soe.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jft.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bib.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eae.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://ena.yj202588.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gtx.ivvv.top

PHP:  file_exists("a.txt");
来源：http://vat.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://pcg.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://gxj.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ubf.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pml.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://bov.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://wyi.zycfv.cn

[F06] 删除文件
来源：http://wsq.vqdsnc.cn

Py:   os.remove("a.txt")
来源：http://qbc.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://ctc.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://mmg.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nju.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uid.yanxiufei.cn

Go:   os.Remove("a.txt")
来源：http://wcs.316326.xyz

Ruby: File.delete("a.txt")
来源：http://pqb.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://uwf.cheryme.top

[F07] 创建目录（含多级）
来源：http://ozx.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aoi.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nke.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tcz.gogol.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lnx.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aaz.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://erd.yj20258888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://edl.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lle.bjfxy.top

[F08] 遍历目录
来源：http://qmu.0kj1m.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lad.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jcy.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://dqh.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://jqc.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pbc.52xcode.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gam.pycfn.com

Ruby: Dir.children("dir")
来源：http://pxu.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://ahi.shangyingyoupin.top

[F09] 获取文件大小
来源：http://wib.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://nsr.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://zil.sjlbkw.cn

JS:   fs.statSync("a.txt").size
来源：http://pbm.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://mmf.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://bic.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://egl.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://rgq.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://pyz.bbcook.cn

[F10] 取文件扩展名 / 文件名
来源：http://jas.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ney.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://poc.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ddh.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://nto.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gmq.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pyl.hcnkem.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qed.jinyuanbaomall.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rvt.shzxlz.cn

[F11] 复制与移动文件
来源：http://kuo.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://leb.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://itn.mhx1999.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://akm.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://moz.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mrr.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ptx.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ofu.gotoacloud.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uth.svipenyu.cn

[F12] CSV 读写
来源：http://bmf.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pdg.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vmh.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ryl.vqdsnc.cn

TS:   // 同上
来源：http://pui.fzhhl.top


<!-- 参考信息 -->