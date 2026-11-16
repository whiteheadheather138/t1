代发 wailian999

================================================================================
来源：http://jyi.smart0.xyz

E. 字符串处理
来源：http://nas.sxryk.cn

================================================================================
来源：http://glc.tian-w.cn

[E01] 拼接字符串
来源：http://bqd.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://snl.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zyk.bjfxy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jne.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lbp.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fbx.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fqf.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://etv.yj20258.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eyb.wangdashe.top

[E02] 重复字符串
来源：http://lhb.zhoulong.xyz

Py:   "ab" * 3
来源：http://grq.jinyuanbaomall.cn

PHP:  str_repeat("ab", 3);
来源：http://qjo.tarul.cn

JS:   "ab".repeat(3)
来源：http://chm.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://nwk.c1oappe.top

Java: "ab".repeat(3)
来源：http://sat.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://xgj.svipenyu.cn

Ruby: "ab" * 3
来源：http://bln.bjfxy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bsd.ybcxt.top

[E03] 截取子串
来源：http://jhn.tianlin.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pae.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mfm.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fvh.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://zmf.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://jwg.guowangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://msz.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://zlo.fanxiaobao.xyz

C#:   s.Substring(1, 3)
来源：http://dwy.jqgfzy.top

[E04] 查找子串位置
来源：http://zio.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://udj.sjlbkw.cn

PHP:  strpos($s, "x");
来源：http://qjm.cheryme.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mqy.316326.xyz

TS:   s.indexOf("x")
来源：http://ewl.316326.xyz

Java: s.indexOf("x")
来源：http://tzc.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://cms.pycfn.com

Ruby: s.index("x")
来源：http://kem.yueranfly.top

C#:   s.IndexOf("x")
来源：http://jas.mhx1999.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vih.zycfv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dgs.sufxvd.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dsa.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kvu.gzhubu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vyk.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zbn.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rdy.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fxj.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xfn.smart0.xyz

[E06] 替换子串
来源：http://uuc.zhixingplan.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wql.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://kmx.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://omd.ivvv.top

TS:   s.replaceAll("a", "b")
来源：http://tfv.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rwm.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zow.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yll.xuanzx.com

C#:   s.Replace("a", "b")
来源：http://zcp.tanke756.top

[E07] 按分隔符拆分
来源：http://ggg.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sfn.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://itq.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nqk.jinqigfzy.top

TS:   s.split(",")
来源：http://bnp.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://onr.zhixingplan.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://awp.yonumen.top

Ruby: s.split(",");  s.split
来源：http://qkl.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pio.cheryme.top

[E08] 数组按分隔符合并
来源：http://fhy.xuanzx.com

Py:   ",".join(items)
来源：http://vdw.sufxvd.cn

PHP:  implode(",", $items);
来源：http://jus.hammf.cn

JS:   items.join(",")
来源：http://vft.fanxiaobao.xyz

TS:   items.join(",")
来源：http://hka.quarkkingdee.top

Java: String.join(",", items)
来源：http://gjh.haohaochexian.top

Go:   strings.Join(items, ",")
来源：http://cfx.pengpengdd.cyou

Ruby: items.join(",")
来源：http://mvh.sufxvd.cn

C#:   string.Join(",", items)
来源：http://yxk.yuxming.cn

[E09] 去除所有空白字符
来源：http://uyf.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://stl.sjlbkw.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dey.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://tpd.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://mdr.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://epn.haohaochexian.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://urq.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://izs.iojbl.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eas.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://duy.daria6918.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ojk.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tsh.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://uuj.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://psy.hywenlv.cn

Java: String.format("%03d", 7)
来源：http://zbz.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://yoz.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fej.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mgl.shanyushiyangkeji.top

[E11] 反转字符串
来源：http://ccw.ywan-chungtsiang.top

Py:   s[::-1]
来源：http://diz.gaohongyu789.top

PHP:  strrev($s);
来源：http://myz.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://gek.cashguo.top

TS:   [...s].reverse().join("")
来源：http://maw.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ojq.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dpo.kuanghao11.cn

Ruby: s.reverse
来源：http://nrj.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://gqn.iojbl.cn

[E12] 统计某字符出现次数
来源：http://naw.xuetiantiany.cn

Py:   s.count("a")
来源：http://odl.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://mhy.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://wlt.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://yxl.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qfi.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://spt.ydzc1.top

Ruby: s.count("a")
来源：http://vcf.shuidangran.top

C#:   s.Count(c => c == 'a')
来源：http://aet.ywan-chungtsiang.top

[E13] 逐字符遍历
来源：http://xws.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://ndv.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hkk.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://xqk.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wjm.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hbc.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://inv.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://gac.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hbk.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://ajr.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bud.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vxt.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cmu.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hwp.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nvv.wangdashe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mpn.jyoumei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mzi.xingfuxueyuan.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wdn.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://ais.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ieh.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ojy.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ghn.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://diq.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mky.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gtu.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://epi.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://amk.yj20258.top

[E16] 数字千分位
来源：http://itl.bbcook.cn

Py:   f"{1234567:,}"
来源：http://xbr.daxiang520.top

PHP:  number_format(1234567);
来源：http://kvn.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xgv.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cqm.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://crr.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sho.yvedp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://erl.zycfv.cn

C#:   1234567.ToString("N0")
来源：http://mor.316326.xyz

[E17] 首字母大写
来源：http://tvd.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://clw.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ubw.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iyf.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dhn.xingfuxueyuan.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nyw.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zlp.bjfxy.top

Ruby: s.capitalize
来源：http://kco.hfpthk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ayw.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://izb.gotoacloud.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rhm.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ixu.hnxiangtu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pdw.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ixr.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fvu.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pmp.guannengcc.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mac.xinyue.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ywa.daria6918.cn

[E19] 多行文本按行拆分
来源：http://bjd.yanxiufei.cn

Py:   s.splitlines()
来源：http://dsu.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cwj.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://mgo.ctjpmb.com

TS:   s.split(/\r?\n/)
来源：http://jqz.ppjwa.cn

Java: s.lines().toList()
来源：http://nle.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://isd.yueranfly.top

Ruby: s.lines
来源：http://zqj.yj20258.top

C#:   s.Split('\n')
来源：http://wjj.xinyue.icu

[E20] 判断字符串是否为空
来源：http://ddz.jyoumei.cn

Py:   if not s:
来源：http://fpz.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eei.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tzt.yfazqb.com

TS:   if (s === "") {}
来源：http://wsl.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://vbg.shangyingyoupin.top

Go:   if s == "" {}
来源：http://nmj.jiagoushi.top

Ruby: if s.empty?
来源：http://tts.xingfuxueyuan.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://chj.cheryme.top

[E21] 超长截断加省略号
来源：http://tdl.fengsongda.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wyo.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rlr.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hyo.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ywn.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ibv.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://dow.52xcode.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yuv.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://odj.aizwys.cn

[E22] 字节长度与字符长度
来源：http://mle.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cxo.sxryk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dgd.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zde.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cdx.yuanzhike.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vmm.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zyc.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://gda.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vkv.dianchejie.cn

================================================================================
来源：http://kxq.sxryk.cn

F. 文件与目录
来源：http://ygi.fengsongda.top

================================================================================
来源：http://dag.bbcook.cn

[F01] 读取整个文件
来源：http://ubh.fanxiaobao.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://way.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://zkw.kuanghao11.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dzz.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fcv.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jaw.sufxvd.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hpd.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://gro.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://qka.fktsv.cn

[F02] 逐行读取文件
来源：http://sae.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hff.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://czm.jiagoushi.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jkt.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pmo.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aur.jqgfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sew.hammf.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://drd.hnqzz.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qpa.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://mjr.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kft.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dey.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://trb.hysaishi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xzr.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tsk.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gsa.xuanzx.com

Ruby: File.write("a.txt", "hi")
来源：http://kai.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ykz.cqqwz.cn

[F04] 追加写入文件
来源：http://nah.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dmz.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kam.feifeiyinyue.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oyg.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vqe.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://htm.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ajy.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xfy.iojbl.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://riz.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://fwl.gzhubu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jug.cashguo.top

PHP:  file_exists("a.txt");
来源：http://zjb.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://xew.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://jhq.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://qra.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dwx.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://nus.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://nsi.yonumen.top

[F06] 删除文件
来源：http://nut.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://eac.316326.xyz

PHP:  unlink("a.txt");
来源：http://oqp.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nhm.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://izk.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xoe.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://zhy.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://zyk.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://upq.tian-w.cn

[F07] 创建目录（含多级）
来源：http://bor.316326.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kic.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://twi.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cca.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gui.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rnt.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rpk.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wjv.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nxg.jianghu66.top

[F08] 遍历目录
来源：http://iqm.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yrc.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zqd.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://hru.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://ocz.fengsongda.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ujy.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://scu.ehwqpu.com

Ruby: Dir.children("dir")
来源：http://wrf.sysykeji.top

C#:   Directory.GetFiles("dir")
来源：http://bvj.yueranfly.top

[F09] 获取文件大小
来源：http://qqm.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://xxm.daria6918.cn

PHP:  filesize("a.txt");
来源：http://mex.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://dbn.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://kri.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cxp.hcnkem.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vpw.hcnkem.com

Ruby: File.size("a.txt")
来源：http://vpi.nanxuanxn.top

C#:   new FileInfo("a.txt").Length
来源：http://fis.hnxiangtu.top

[F10] 取文件扩展名 / 文件名
来源：http://usy.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iyx.yangfankeji.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qmm.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://arw.smart0.xyz

TS:   path.extname("a.txt")
来源：http://itm.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rbx.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uif.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ain.iojbl.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hkg.sxryk.cn

[F11] 复制与移动文件
来源：http://qhj.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dpr.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hjt.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vrr.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yni.quarkkingdee.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://elx.hnqzz.top


<!-- 参考信息 -->