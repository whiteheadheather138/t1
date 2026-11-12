代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://pcm.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://byl.xuanzx.com

JS:   arr.join(", ")
来源：http://bah.yuxming.cn

TS:   arr.join(", ")
来源：http://kqy.zhoulong.xyz

Java: String.join(", ", list)
来源：http://mjq.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://kct.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://xul.tarul.cn

C#:   string.Join(", ", list)
来源：http://xxu.gogol.net.cn

================================================================================
来源：http://svv.jianghu66.top

E. 字符串处理
来源：http://ral.pycfn.com

================================================================================
来源：http://xvi.pycfn.com

[E01] 拼接字符串
来源：http://wpp.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gaw.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dpu.chenlongwang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gqx.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xaw.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hod.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ebj.hammf.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ose.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ovl.gogol.net.cn

[E02] 重复字符串
来源：http://zpk.yfazqb.com

Py:   "ab" * 3
来源：http://mta.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://lal.cdnleiting.top

JS:   "ab".repeat(3)
来源：http://iyh.bjfxy.top

TS:   "ab".repeat(3)
来源：http://ogo.yfazqb.com

Java: "ab".repeat(3)
来源：http://xft.yongpay.top

Go:   strings.Repeat("ab", 3)
来源：http://tgo.sxryk.cn

Ruby: "ab" * 3
来源：http://gel.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rsu.yfazqb.com

[E03] 截取子串
来源：http://gfi.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kxb.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ybo.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hqo.yj20258.top

TS:   s.slice(1, 4)
来源：http://pur.iojbl.cn

Java: s.substring(1, 4)
来源：http://dfp.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hgi.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://ceh.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://eoy.pycfn.com

[E04] 查找子串位置
来源：http://azv.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://ses.tanke756.top

PHP:  strpos($s, "x");
来源：http://rbf.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jlj.fktsv.cn

TS:   s.indexOf("x")
来源：http://gdd.c1oappe.top

Java: s.indexOf("x")
来源：http://lbk.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://lab.iojbl.cn

Ruby: s.index("x")
来源：http://vps.tian-w.cn

C#:   s.IndexOf("x")
来源：http://uvg.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wus.bbcook.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ulm.zdqjudy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://phq.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://svz.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://uqo.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://caw.wangdashe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qji.zhengqikj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tnp.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tbv.zhengqikj.top

[E06] 替换子串
来源：http://seg.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xao.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://cks.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zgf.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://eeo.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://idg.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vur.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pvp.aibaodan.cn

C#:   s.Replace("a", "b")
来源：http://hdo.yuxming.cn

[E07] 按分隔符拆分
来源：http://ndj.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vfj.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xmc.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nlx.zhengqikj.top

TS:   s.split(",")
来源：http://lzq.ybcxt.top

Java: s.split(",");  s.split("\\s+")
来源：http://gaj.quarkkingdee.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qix.cheryme.top

Ruby: s.split(",");  s.split
来源：http://txt.havefunace.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jem.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://hld.yvedp.cn

Py:   ",".join(items)
来源：http://wxk.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://nnb.smart0.xyz

JS:   items.join(",")
来源：http://kcr.zdqjudy.top

TS:   items.join(",")
来源：http://jpy.shzxlz.cn

Java: String.join(",", items)
来源：http://lmv.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://bkk.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://gmd.redwolf501.top

C#:   string.Join(",", items)
来源：http://sqc.cdnleiting.top

[E09] 去除所有空白字符
来源：http://cog.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ewm.fzhhl.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mmn.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://ulb.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://gew.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://xyd.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://fut.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://obt.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ztf.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://uzc.shanyushiyangtech.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://enu.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jxy.jinyuanbaomall.cn

JS:   "7".padStart(3, "0")
来源：http://efh.shzxlz.cn

TS:   "7".padStart(3, "0")
来源：http://wbo.fzhhl.top

Java: String.format("%03d", 7)
来源：http://whj.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yzr.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ylw.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hip.shzxlz.cn

[E11] 反转字符串
来源：http://nqn.jinqigfzy.top

Py:   s[::-1]
来源：http://zvy.tanke756.top

PHP:  strrev($s);
来源：http://dcr.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://rvu.bbcook.cn

TS:   [...s].reverse().join("")
来源：http://nlk.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gog.hfpthk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rgq.xziqi.cn

Ruby: s.reverse
来源：http://lsq.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gqq.yongpay.top

[E12] 统计某字符出现次数
来源：http://ksf.52xcode.cn

Py:   s.count("a")
来源：http://evk.ydjk.org.cn

PHP:  substr_count($s, "a");
来源：http://fky.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://vob.yj202588.top

TS:   s.split("a").length - 1
来源：http://aka.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zua.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://icz.meibo888.top

Ruby: s.count("a")
来源：http://abd.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://ror.hywenlv.cn

[E13] 逐字符遍历
来源：http://vra.sweek.top

Py:   for ch in s: print(ch)
来源：http://rlp.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qrd.wangdashe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ddg.fzhhl.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cag.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zuh.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rtr.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nur.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://evx.zhixingplan.top

[E14] URL 编码与 Base64
来源：http://abq.hfpthk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://whu.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://hui.yj20258.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://orp.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uch.sweek.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xdy.hammf.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zut.guowangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gkm.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hie.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://pji.epnwcf.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ijq.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qrd.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dxg.yj202588.top

TS:   // 同上，务必做 XSS 过滤
来源：http://arb.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rrj.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wyu.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mqs.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zmu.bbcook.cn

[E16] 数字千分位
来源：http://ces.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://ukt.sufxvd.cn

PHP:  number_format(1234567);
来源：http://czw.dashuyun.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vok.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://czx.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qkw.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kdh.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://brh.hammf.cn

C#:   1234567.ToString("N0")
来源：http://ynx.haohaochexian.top

[E17] 首字母大写
来源：http://xnn.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ybx.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dhq.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zul.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sfn.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eep.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ume.zhijiandao.cn

Ruby: s.capitalize
来源：http://axn.daria6918.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ydy.jqgfzy.top

[E18] 模板占位符替换
来源：http://tnt.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wpz.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://csu.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tte.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fhg.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lkd.ppjwa.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hnf.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ymm.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qal.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://lql.shangyingyoupin.top

Py:   s.splitlines()
来源：http://vlp.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mry.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://jif.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://cdb.hnxiangtu.top

Java: s.lines().toList()
来源：http://xbb.jinyuanbaomall.cn

Go:   strings.Split(s, "\n")
来源：http://yne.shzxlz.cn

Ruby: s.lines
来源：http://qoc.zdqjudy.top

C#:   s.Split('\n')
来源：http://mzg.sweek.top

[E20] 判断字符串是否为空
来源：http://mes.gaohongyu789.top

Py:   if not s:
来源：http://pby.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://idq.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qzg.zhengqikj.top

TS:   if (s === "") {}
来源：http://xak.iojbl.cn

Java: if (s.isEmpty()) {}
来源：http://wve.bbcook.cn

Go:   if s == "" {}
来源：http://rqp.ppjwa.cn

Ruby: if s.empty?
来源：http://udo.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xys.yuxming.cn

[E21] 超长截断加省略号
来源：http://agb.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kdc.daria6918.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lno.haohaochexian.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kzp.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dfx.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mnp.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://hrt.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wxd.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kte.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://eob.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wrb.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ako.yanxiufei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jul.gotoacloud.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jkp.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pue.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pmn.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://rhp.zdbjq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kqc.jqgfzy.top

================================================================================
来源：http://xhd.cucudq.cn

F. 文件与目录
来源：http://jkk.hywenlv.cn

================================================================================
来源：http://cib.zdbjq.cn

[F01] 读取整个文件
来源：http://aht.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dsh.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://vfj.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zte.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yph.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://twu.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nsk.tian-w.cn

Ruby: File.read("a.txt")
来源：http://pmb.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://kct.yj20258888.top

[F02] 逐行读取文件
来源：http://vhw.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kun.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://imz.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nqd.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fgk.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qof.tian-w.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vzp.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rcl.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ygc.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://qys.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nyv.zhixingplan.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://czj.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://had.yonumen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cfy.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bps.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ryu.jlsjyb.cn

Ruby: File.write("a.txt", "hi")
来源：http://bpq.9152youxi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zzc.ctjpmb.com

[F04] 追加写入文件
来源：http://wyg.hnqzz.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tlt.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hxu.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hzq.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://txr.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://esz.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lcy.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mzn.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://udz.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://bmk.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ksa.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://wyc.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://lnl.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://qjb.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://czt.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rfn.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://tqy.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://hde.dianchejie.cn

[F06] 删除文件
来源：http://sxt.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://ijg.andypj.xyz

PHP:  unlink("a.txt");
来源：http://fll.tarul.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tdx.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://asc.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uee.yj20258.top

Go:   os.Remove("a.txt")
来源：http://ntf.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://dci.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://qbu.tarul.cn

[F07] 创建目录（含多级）
来源：http://hkc.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rsz.zhoulong.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://avo.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qaq.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://udn.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://emw.nanxuanxn.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jvh.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oxf.fengsongda.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://heh.gotoacloud.top

[F08] 遍历目录
来源：http://cgj.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tsl.nanxinkj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sou.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://ndp.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://oly.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zug.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dnb.bjfxy.top

Ruby: Dir.children("dir")
来源：http://xdi.zhaomingkeji.xyz

C#:   Directory.GetFiles("dir")
来源：http://zqo.sweek.top

[F09] 获取文件大小
来源：http://cbk.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://tdm.zycfv.cn

PHP:  filesize("a.txt");
来源：http://amg.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://jbm.yanxiufei.cn

TS:   fs.statSync("a.txt").size
来源：http://ozd.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://tiy.yueranfly.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tjb.yonumen.top

Ruby: File.size("a.txt")
来源：http://jlx.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://sie.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://acq.feifeiyinyue.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dey.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cof.pengpengdd.cyou

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sar.yj20258888.top

TS:   path.extname("a.txt")
来源：http://xsy.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kcz.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lmz.mhx1999.top


<!-- 参考信息 -->