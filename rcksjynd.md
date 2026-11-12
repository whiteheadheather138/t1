代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://syq.sweek.top

PHP:  implode(", ", $arr);
来源：http://bhw.fzhhl.top

JS:   arr.join(", ")
来源：http://ayw.bbcook.cn

TS:   arr.join(", ")
来源：http://ysg.jqgfzy.top

Java: String.join(", ", list)
来源：http://xni.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://mza.cheryme.top

Ruby: arr.join(", ")
来源：http://brj.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://too.dashuyun.cn

================================================================================
来源：http://cxc.zhengqikj.top

E. 字符串处理
来源：http://iso.fanxiaobao.xyz

================================================================================
来源：http://wja.cashguo.top

[E01] 拼接字符串
来源：http://thp.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bje.yj20258888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fhu.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://amd.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ivf.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://axm.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jbp.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yzk.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hkl.sysykeji.top

[E02] 重复字符串
来源：http://mwa.xuetiantiany.cn

Py:   "ab" * 3
来源：http://zek.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://gso.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://nwz.yuxming.cn

TS:   "ab".repeat(3)
来源：http://eiw.sysykeji.top

Java: "ab".repeat(3)
来源：http://onv.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://raz.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://vxu.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://msv.xuetiantiany.cn

[E03] 截取子串
来源：http://jla.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mnb.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ulv.gogol.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nhr.cdnleiting.top

TS:   s.slice(1, 4)
来源：http://qgj.cucudq.cn

Java: s.substring(1, 4)
来源：http://cwl.ybcxt.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rzy.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sai.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://cst.yanxiufei.cn

[E04] 查找子串位置
来源：http://ecx.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://lvs.dashuyun.cn

PHP:  strpos($s, "x");
来源：http://wwc.hongshengwenyu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pkq.cqqwz.cn

TS:   s.indexOf("x")
来源：http://zxx.c1oappe.top

Java: s.indexOf("x")
来源：http://txb.yj20258888.top

Go:   strings.Index(s, "x")
来源：http://two.chenjidiqi.icu

Ruby: s.index("x")
来源：http://fpz.hnxiangtu.top

C#:   s.IndexOf("x")
来源：http://iba.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://qcv.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bho.sysykeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vzd.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://imd.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gsi.jyoumei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ivv.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://skw.aizwys.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ncn.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ssl.ppjwa.cn

[E06] 替换子串
来源：http://hwm.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qch.cashguo.top

PHP:  str_replace("a", "b", $s);
来源：http://len.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ahl.wangshuangyany.cn

TS:   s.replaceAll("a", "b")
来源：http://inw.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://idw.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xev.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://whs.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://gux.yueranfly.top

[E07] 按分隔符拆分
来源：http://qtd.hfpthk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xgs.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oqd.yj20258.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vmu.nwbrower.top

TS:   s.split(",")
来源：http://len.wangshuangyany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ydm.shanyushiyangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tef.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://lnb.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mmq.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://znc.gotoacloud.top

Py:   ",".join(items)
来源：http://fru.chenzaomai.com

PHP:  implode(",", $items);
来源：http://wyl.pycfn.com

JS:   items.join(",")
来源：http://aqt.dianchejie.cn

TS:   items.join(",")
来源：http://zyd.gogol.net.cn

Java: String.join(",", items)
来源：http://dkz.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://gxg.daxiang520.top

Ruby: items.join(",")
来源：http://jjk.yj20258.top

C#:   string.Join(",", items)
来源：http://mdb.hcnkem.com

[E09] 去除所有空白字符
来源：http://xob.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mji.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wjm.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://dnt.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://vzc.gotoacloud.top

Java: s.replaceAll("\\s+", "")
来源：http://eyv.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zpk.bjfxy.top

Ruby: s.gsub(/\s+/, "")
来源：http://vlf.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yxm.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://roh.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mgg.yongpay.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ath.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://ucy.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://fyj.daxiang520.top

Java: String.format("%03d", 7)
来源：http://yfj.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://dij.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qfu.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sdl.nanxuanxn.top

[E11] 反转字符串
来源：http://jra.feifeiyinyue.top

Py:   s[::-1]
来源：http://pmx.gogol.net.cn

PHP:  strrev($s);
来源：http://gmk.guannengcc.top

JS:   [...s].reverse().join("")
来源：http://dvl.sxryk.cn

TS:   [...s].reverse().join("")
来源：http://rfs.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://psf.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uuh.dashuyun.cn

Ruby: s.reverse
来源：http://rwp.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://onb.52xcode.cn

[E12] 统计某字符出现次数
来源：http://mwb.tanke756.top

Py:   s.count("a")
来源：http://dwx.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://azf.nwbrower.top

JS:   s.split("a").length - 1
来源：http://ccu.xuanzx.com

TS:   s.split("a").length - 1
来源：http://qwr.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://emj.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://brm.xuanzx.com

Ruby: s.count("a")
来源：http://vft.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://lqz.zhoulong.xyz

[E13] 逐字符遍历
来源：http://vsi.yj202588.top

Py:   for ch in s: print(ch)
来源：http://jip.daxiang520.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://git.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ndg.hammf.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bwr.yongpay.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tqp.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vur.guannengcc.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iau.shangyingyoupin.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tnu.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://cxj.nanxinkj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://min.yonumen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://eet.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cgn.nanxinkj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wwg.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tlm.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hld.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kbj.chenjidiqi.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pwl.kuanghao11.cn

[E15] HTML 转义 / 反转义
来源：http://haz.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qvn.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nan.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eiw.cheryme.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vfb.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ofm.fktsv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jkl.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lvi.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lxz.zhijiandao.cn

[E16] 数字千分位
来源：http://ydm.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://gaw.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://ufa.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vrz.hcnkem.com

TS:   (1234567).toLocaleString("en-US")
来源：http://uds.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wgn.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dan.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nfk.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://bog.ydjk.org.cn

[E17] 首字母大写
来源：http://vzl.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://adi.zdbjq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tur.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vxv.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kmv.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vrj.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zkd.yuanzhike.top

Ruby: s.capitalize
来源：http://gap.52xcode.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xel.yj202588.top

[E18] 模板占位符替换
来源：http://tkr.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://quk.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hah.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fsh.yvedp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fol.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zjz.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wqy.jqgufenzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cmm.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ezq.316326.xyz

[E19] 多行文本按行拆分
来源：http://qtg.jqgufenzy.top

Py:   s.splitlines()
来源：http://vls.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zae.birdmap.top

JS:   s.split(/\r?\n/)
来源：http://uni.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://rnc.pengpengdd.cyou

Java: s.lines().toList()
来源：http://xyu.zdqjudy.top

Go:   strings.Split(s, "\n")
来源：http://ojw.chenlongwang.top

Ruby: s.lines
来源：http://dfk.meibo888.top

C#:   s.Split('\n')
来源：http://fbx.pycfn.com

[E20] 判断字符串是否为空
来源：http://ohs.zhixingplan.top

Py:   if not s:
来源：http://mfe.jinyuanbaomall.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zsm.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xuw.iojbl.cn

TS:   if (s === "") {}
来源：http://tor.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://urs.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://bsp.fehbvm.com

Ruby: if s.empty?
来源：http://tfe.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zye.0kj1m.cn

[E21] 超长截断加省略号
来源：http://oso.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uae.bbcook.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://def.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bqi.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ofy.cashguo.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oui.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://iaq.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tsk.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://voa.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://btq.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nzt.chenzaomai.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jof.xziqi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://byk.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nnj.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bht.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rhz.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://jnp.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bzd.svipenyu.cn

================================================================================
来源：http://gfn.hesvh.cn

F. 文件与目录
来源：http://xjc.gzhubu.top

================================================================================
来源：http://ogj.yj202588.top

[F01] 读取整个文件
来源：http://def.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gnk.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://rfw.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nxb.smart0.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eue.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tlv.jianghu66.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pqx.uphjek.com

Ruby: File.read("a.txt")
来源：http://fwt.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://omv.ppjwa.cn

[F02] 逐行读取文件
来源：http://toy.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wwd.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sjo.aizwys.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ygj.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yui.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dno.yfazqb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://btj.hfpthk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kfn.shangyingyoupin.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tyi.tarul.cn

[F03] 写入文件（覆盖）
来源：http://jqi.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aot.zdqjudy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pak.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rbc.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ony.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eip.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zli.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://xsc.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aqq.gzhubu.top

[F04] 追加写入文件
来源：http://esh.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xoc.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eua.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wur.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kas.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lnj.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ayi.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jjp.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wkd.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://mmk.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tgi.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://jht.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://icd.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://qed.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ffd.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uoi.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://khj.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://oed.zhijiandao.cn

[F06] 删除文件
来源：http://agw.yj20258.top

Py:   os.remove("a.txt")
来源：http://rys.jinghuilouyu.cn

PHP:  unlink("a.txt");
来源：http://tbl.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://hdf.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://nth.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mzb.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://knw.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://abb.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://jut.xinyue.icu

[F07] 创建目录（含多级）
来源：http://tpp.tianlin.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bmm.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tvq.snrcjt.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eym.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fmq.pengpengdd.cyou

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tcp.birdmap.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mpy.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bew.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hly.svipenyu.cn

[F08] 遍历目录
来源：http://nzg.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://zbl.yj202588.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gtt.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://uiq.cashguo.top

TS:   fs.readdirSync("dir")
来源：http://tms.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hcr.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zmt.yvedp.cn

Ruby: Dir.children("dir")
来源：http://qfx.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://ynd.yongpay.top

[F09] 获取文件大小
来源：http://ybe.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://fml.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://udp.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://amq.tian-w.cn

TS:   fs.statSync("a.txt").size
来源：http://hfk.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yln.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mju.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://yvu.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://yje.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://ysq.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://syn.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://clo.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lvk.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://dia.hesvh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bio.yj202588.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://clh.daria6918.cn


<!-- 参考信息 -->