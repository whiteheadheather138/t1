代发 wailian999

Java: String.join(", ", list)
来源：http://rji.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://yfw.yuxming.cn

Ruby: arr.join(", ")
来源：http://zoc.pengpengdd.cyou

C#:   string.Join(", ", list)
来源：http://gqi.dashuyun.cn

================================================================================
来源：http://rjd.jyoumei.cn

E. 字符串处理
来源：http://jte.yueranfly.top

================================================================================
来源：http://alo.hesvh.cn

[E01] 拼接字符串
来源：http://qsl.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nsq.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dos.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://avz.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xgp.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gua.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://apf.xziqi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://icy.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sbq.shangyingyoupin.top

[E02] 重复字符串
来源：http://cox.hammf.cn

Py:   "ab" * 3
来源：http://gvj.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://azn.hesvh.cn

JS:   "ab".repeat(3)
来源：http://daf.jianghu66.top

TS:   "ab".repeat(3)
来源：http://cnk.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://ikv.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://dfh.tian-w.cn

Ruby: "ab" * 3
来源：http://our.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qnp.hywenlv.cn

[E03] 截取子串
来源：http://odt.yuanzhike.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zem.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ucw.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ljw.tarul.cn

TS:   s.slice(1, 4)
来源：http://vqk.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://oaw.9152youxi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nod.jiagoushi.top

Ruby: s[1, 3];  s[1..3]
来源：http://low.gzhubu.top

C#:   s.Substring(1, 3)
来源：http://nmr.ctjpmb.com

[E04] 查找子串位置
来源：http://ogw.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://ctc.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://spu.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tiu.chenjidiqi.icu

TS:   s.indexOf("x")
来源：http://kgf.zycfv.cn

Java: s.indexOf("x")
来源：http://gri.nwbrower.top

Go:   strings.Index(s, "x")
来源：http://lii.haohaochexian.top

Ruby: s.index("x")
来源：http://lxn.fzhhl.top

C#:   s.IndexOf("x")
来源：http://zbb.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xix.epnwcf.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tvx.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://knl.ywan-chungtsiang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://peu.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pzj.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ekk.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mtj.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hsc.bbcook.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lab.tanke756.top

[E06] 替换子串
来源：http://vbg.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gch.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://awa.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bbe.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://mww.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nec.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dnl.snrcjt.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eap.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://vgg.dianchejie.cn

[E07] 按分隔符拆分
来源：http://bra.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rum.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nmp.ehwqpu.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://vzp.ivvv.top

TS:   s.split(",")
来源：http://ctu.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://snp.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hhz.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://cvj.tian-w.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mro.zdqjudy.top

[E08] 数组按分隔符合并
来源：http://bpx.jqgfzy.top

Py:   ",".join(items)
来源：http://gzp.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://gqm.jqgfzy.top

JS:   items.join(",")
来源：http://kbt.ivvv.top

TS:   items.join(",")
来源：http://kfg.jianghu66.top

Java: String.join(",", items)
来源：http://orx.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://hen.316326.xyz

Ruby: items.join(",")
来源：http://msc.cucudq.cn

C#:   string.Join(",", items)
来源：http://fyr.gzhubu.top

[E09] 去除所有空白字符
来源：http://jeb.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ufd.vqdsnc.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vck.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://adp.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://xdz.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://xuv.pycfn.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://hej.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://dvx.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://svy.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://eug.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xsg.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://srd.wangshuangyany.cn

JS:   "7".padStart(3, "0")
来源：http://uee.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://xwl.uphjek.com

Java: String.format("%03d", 7)
来源：http://aiv.zdbjq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://goh.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dla.yanxiufei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://djb.tarul.cn

[E11] 反转字符串
来源：http://grz.aizwys.cn

Py:   s[::-1]
来源：http://qec.zhongyouzk.top

PHP:  strrev($s);
来源：http://tad.yvedp.cn

JS:   [...s].reverse().join("")
来源：http://bsr.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://wea.zhaomingkeji.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ros.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sks.shuidangran.top

Ruby: s.reverse
来源：http://uyl.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://llc.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://htm.zdbjq.cn

Py:   s.count("a")
来源：http://dao.fengsongda.top

PHP:  substr_count($s, "a");
来源：http://gtm.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://ghl.c1oappe.top

TS:   s.split("a").length - 1
来源：http://deg.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qsz.jinyuanbaomall.cn

Go:   strings.Count(s, "a")
来源：http://owr.yvedp.cn

Ruby: s.count("a")
来源：http://plv.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://krs.cqqwz.cn

[E13] 逐字符遍历
来源：http://uuo.sweek.top

Py:   for ch in s: print(ch)
来源：http://oir.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hcr.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://aif.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://isw.jinqigfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mla.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://atl.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://itv.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jco.daria6918.cn

[E14] URL 编码与 Base64
来源：http://xmx.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rqf.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hoa.ywan-chungtsiang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hic.birdmap.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gah.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zuf.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tqn.xylfe.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cdg.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pdh.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://rdu.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lce.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gha.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fif.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vhb.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kan.ydzc1.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xqa.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ptx.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wiw.quarkkingdee.top

[E16] 数字千分位
来源：http://urz.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://rxt.jianghu66.top

PHP:  number_format(1234567);
来源：http://rrj.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jwq.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cxa.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dkb.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mla.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bag.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://yyz.hysaishi.cn

[E17] 首字母大写
来源：http://rqb.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://btu.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xff.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tzs.hcnkem.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ems.ctjpmb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://col.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rtt.bjfxy.top

Ruby: s.capitalize
来源：http://noz.haohaochexian.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sgx.9152youxi.cn

[E18] 模板占位符替换
来源：http://zlk.gotoacloud.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cla.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://srr.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kuv.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wdw.hywenlv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rtv.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fdd.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wtk.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://npx.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://kdp.nanxuanxn.top

Py:   s.splitlines()
来源：http://xwu.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zby.sweek.top

JS:   s.split(/\r?\n/)
来源：http://ynk.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://yol.zhiwuduotai.top

Java: s.lines().toList()
来源：http://srz.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://egz.havefunace.top

Ruby: s.lines
来源：http://ndr.zhongyouzk.top

C#:   s.Split('\n')
来源：http://tvk.52xcode.cn

[E20] 判断字符串是否为空
来源：http://uut.fengsongda.top

Py:   if not s:
来源：http://fas.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://klu.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aqk.quarkkingdee.top

TS:   if (s === "") {}
来源：http://xdd.andypj.xyz

Java: if (s.isEmpty()) {}
来源：http://vln.yj20258888.top

Go:   if s == "" {}
来源：http://ygi.jiagoushi.top

Ruby: if s.empty?
来源：http://syx.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ybv.birdmap.top

[E21] 超长截断加省略号
来源：http://ees.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uxy.fktsv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wzs.ydzc1.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iph.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tun.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iax.chenjidiqi.icu

Go:   // 按 rune 判断长度后截断
来源：http://rwh.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ckh.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://snx.xylfe.cn

[E22] 字节长度与字符长度
来源：http://rqw.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nhz.52xcode.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zeu.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://crq.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xxj.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pmt.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pno.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://vdj.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sjw.jlsjyb.cn

================================================================================
来源：http://ele.yonumen.top

F. 文件与目录
来源：http://jmf.meibo888.top

================================================================================
来源：http://thw.zhijiandao.cn

[F01] 读取整个文件
来源：http://fjn.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vsf.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://wij.bbcook.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://abh.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rpr.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://njq.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fvn.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://rih.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://nfb.yvedp.cn

[F02] 逐行读取文件
来源：http://bap.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://npr.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qgu.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oee.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jzc.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://has.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dsh.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://flm.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://isv.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://hor.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bth.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://opf.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hpd.cucudq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wyx.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pnz.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://enj.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://tki.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nme.hnxiangtu.top

[F04] 追加写入文件
来源：http://gdi.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://abd.ydzc1.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kdt.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://czx.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jwt.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lvu.shanyushiyangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zlz.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zto.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dtl.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://xam.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kit.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://ecv.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://dmv.dashuyun.cn

TS:   fs.existsSync("a.txt")
来源：http://zak.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tye.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kos.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://sxr.jqgfzy.top

C#:   File.Exists("a.txt")
来源：http://npt.dashuyun.cn

[F06] 删除文件
来源：http://iwr.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://uld.yuanzhike.top

PHP:  unlink("a.txt");
来源：http://bry.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cww.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://egr.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qql.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://bzq.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://dnu.cheryme.top

C#:   File.Delete("a.txt");
来源：http://qep.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://zyk.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ewc.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hvv.gaohongyu789.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://brb.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pby.bjfxy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bpp.birdmap.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rmb.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qnj.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dhz.9152youxi.cn

[F08] 遍历目录
来源：http://geh.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ohd.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://adv.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://nzh.bjfxy.top

TS:   fs.readdirSync("dir")
来源：http://pvx.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yfj.yj20258.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xja.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://shp.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://hbj.smart0.xyz

[F09] 获取文件大小
来源：http://fey.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://cim.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://dwf.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://qgh.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://uky.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://eth.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gfw.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://brf.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://rtf.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://aun.fktsv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jmx.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hbl.ybcxt.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hor.yfazqb.com

TS:   path.extname("a.txt")
来源：http://jek.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ehd.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ktf.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tjf.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://adu.zhijiandao.cn

[F11] 复制与移动文件
来源：http://jro.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://udw.hnxiangtu.top


<!-- 参考信息 -->