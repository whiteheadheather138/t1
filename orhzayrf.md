代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fll.jiagoushi.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bdg.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bdc.sjlbkw.cn

[D26] 数组转字符串
来源：http://ydb.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://rvv.meibo888.top

PHP:  implode(", ", $arr);
来源：http://kxp.cashguo.top

JS:   arr.join(", ")
来源：http://uqq.hesvh.cn

TS:   arr.join(", ")
来源：http://smh.nanxinkj.top

Java: String.join(", ", list)
来源：http://inc.zhiwuduotai.top

Go:   strings.Join(strs, ", ")
来源：http://noj.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://zaz.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://hyc.yj20258888.top

================================================================================
来源：http://twh.quarkkingdee.top

E. 字符串处理
来源：http://fdf.xingfuxueyuan.xyz

================================================================================
来源：http://nqp.wangshuangyany.cn

[E01] 拼接字符串
来源：http://msj.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gio.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hqi.ivvv.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uxu.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://okk.tian-w.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://end.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iop.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tdt.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tsh.jlsjyb.cn

[E02] 重复字符串
来源：http://agf.svipenyu.cn

Py:   "ab" * 3
来源：http://ccy.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://gnc.zdqjudy.top

JS:   "ab".repeat(3)
来源：http://xkt.tanke756.top

TS:   "ab".repeat(3)
来源：http://lku.yj20258888.top

Java: "ab".repeat(3)
来源：http://zgb.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://gcd.hysaishi.cn

Ruby: "ab" * 3
来源：http://khn.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://thh.mhx1999.top

[E03] 截取子串
来源：http://efd.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ixl.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rjv.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rcl.andypj.xyz

TS:   s.slice(1, 4)
来源：http://xkx.hcnkem.com

Java: s.substring(1, 4)
来源：http://qhz.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://spt.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vvn.yvedp.cn

C#:   s.Substring(1, 3)
来源：http://abq.zhiwuduotai.top

[E04] 查找子串位置
来源：http://yfk.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://ssw.fehbvm.com

PHP:  strpos($s, "x");
来源：http://gza.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pkf.jyoumei.cn

TS:   s.indexOf("x")
来源：http://vak.hnqzz.top

Java: s.indexOf("x")
来源：http://iiv.yj20258888.top

Go:   strings.Index(s, "x")
来源：http://fxp.jianghu66.top

Ruby: s.index("x")
来源：http://swi.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://yrw.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://knz.zhongyouzk.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iqs.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fec.fengsongda.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://euh.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wtb.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ncf.gaohongyu789.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oqm.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gye.xingfuxueyuan.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tqd.feifeiyinyue.top

[E06] 替换子串
来源：http://atz.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bmf.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://wdr.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lez.xuetiantiany.cn

TS:   s.replaceAll("a", "b")
来源：http://lys.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qfn.pycfn.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mjy.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sgc.chenlongwang.top

C#:   s.Replace("a", "b")
来源：http://wgk.guannengcc.top

[E07] 按分隔符拆分
来源：http://khl.pengpengdd.cyou

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eid.gogol.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wby.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eom.aizwys.cn

TS:   s.split(",")
来源：http://ytz.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hbm.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kcl.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://fza.tianlin.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tqs.sxryk.cn

[E08] 数组按分隔符合并
来源：http://ksd.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://fvw.yonumen.top

PHP:  implode(",", $items);
来源：http://rhq.zdqjudy.top

JS:   items.join(",")
来源：http://uwl.tanke756.top

TS:   items.join(",")
来源：http://lrg.fehbvm.com

Java: String.join(",", items)
来源：http://lvl.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://kto.sjlbkw.cn

Ruby: items.join(",")
来源：http://ksp.yfazqb.com

C#:   string.Join(",", items)
来源：http://nrh.cashguo.top

[E09] 去除所有空白字符
来源：http://btp.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ooj.aibaodan.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yit.hfpthk.cn

JS:   s.replace(/\s+/g, "")
来源：http://klw.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://ruu.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://rqm.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://vhz.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rky.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://srk.xuanzx.com

[E10] 左侧补零 / 定长填充
来源：http://avx.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lkr.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wqa.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://okj.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://yek.xinyue.icu

Java: String.format("%03d", 7)
来源：http://bfc.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vtr.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xmn.zhaomingkeji.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pxe.jlsjyb.cn

[E11] 反转字符串
来源：http://vml.cdnleiting.top

Py:   s[::-1]
来源：http://evk.shanyushiyangtech.top

PHP:  strrev($s);
来源：http://lrs.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://jia.ydjk.org.cn

TS:   [...s].reverse().join("")
来源：http://kvv.jinghuilouyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://efx.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jzp.aibaodan.cn

Ruby: s.reverse
来源：http://jxc.kuanghao11.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oge.andypj.xyz

[E12] 统计某字符出现次数
来源：http://khh.yuanzhike.top

Py:   s.count("a")
来源：http://aoj.hesvh.cn

PHP:  substr_count($s, "a");
来源：http://hzf.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://hzi.jyoumei.cn

TS:   s.split("a").length - 1
来源：http://why.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zdk.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://yns.birdmap.top

Ruby: s.count("a")
来源：http://rwg.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://lda.ehwqpu.com

[E13] 逐字符遍历
来源：http://oxw.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://xfh.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tsl.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://eos.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://iwl.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rbm.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zgj.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://rob.316326.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zos.guannengcc.top

[E14] URL 编码与 Base64
来源：http://bfr.chenlongwang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mcz.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wsk.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rmh.birdmap.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://phs.tanke756.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hlw.zhijiandao.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dst.jinqigufen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cqs.hesvh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://djn.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://jph.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kds.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uax.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uwi.zhengqikj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nsx.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rts.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://swd.ywan-chungtsiang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bfz.zycfv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://duz.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://usu.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://jdx.fengsongda.top

PHP:  number_format(1234567);
来源：http://rod.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zej.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ube.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yja.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vaq.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hyx.zdqjudy.top

C#:   1234567.ToString("N0")
来源：http://kaj.chenlongwang.top

[E17] 首字母大写
来源：http://oos.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iic.jinyuanbaomall.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rue.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ijk.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lyb.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kmx.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cui.jinqigufen.top

Ruby: s.capitalize
来源：http://wnr.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wky.chenzaomai.com

[E18] 模板占位符替换
来源：http://fnf.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qep.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gcv.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vba.wangshuangyany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ibs.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kks.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yyj.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zlp.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jml.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://rti.fktsv.cn

Py:   s.splitlines()
来源：http://oms.iojbl.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cog.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://wzn.wangshuangyany.cn

TS:   s.split(/\r?\n/)
来源：http://aav.52xcode.cn

Java: s.lines().toList()
来源：http://hkq.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://vvw.jiagoushi.top

Ruby: s.lines
来源：http://ifa.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://gdy.havefunace.top

[E20] 判断字符串是否为空
来源：http://gqf.jqgfzy.top

Py:   if not s:
来源：http://usf.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lcq.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mlj.hcnkem.com

TS:   if (s === "") {}
来源：http://scc.zhaomingkeji.xyz

Java: if (s.isEmpty()) {}
来源：http://fvm.jqgufenzy.top

Go:   if s == "" {}
来源：http://afe.sweek.top

Ruby: if s.empty?
来源：http://juc.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rmg.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://gyh.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://edj.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://olq.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://apy.havefunace.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://are.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yia.tarul.cn

Go:   // 按 rune 判断长度后截断
来源：http://szh.zdqjudy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mnq.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sgm.tanke756.top

[E22] 字节长度与字符长度
来源：http://gvz.zdqjudy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://knk.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mcx.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ann.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://txq.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lho.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://koy.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://vzd.bjfxy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pxy.zhoulong.xyz

================================================================================
来源：http://akv.ydjk.org.cn

F. 文件与目录
来源：http://zaf.ywan-chungtsiang.top

================================================================================
来源：http://bqo.jinqigfzy.top

[F01] 读取整个文件
来源：http://phu.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eyg.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://tvn.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sjd.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ahq.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mrv.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mnx.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://rix.jinqigfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://bmi.dianchejie.cn

[F02] 逐行读取文件
来源：http://tuo.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ita.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iot.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aek.meibo888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lht.tarul.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cqf.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bpp.zdqjudy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tzh.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://btp.bbcook.cn

[F03] 写入文件（覆盖）
来源：http://ooe.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://axg.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wes.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jxs.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ozu.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ate.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zkd.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://nxf.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iyh.feifeiyinyue.top

[F04] 追加写入文件
来源：http://ylj.xinyue.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ljb.daria6918.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://frv.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gjz.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nhk.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yjt.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uiq.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nqq.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ugs.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://dwf.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kay.yongpay.top

PHP:  file_exists("a.txt");
来源：http://ros.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://rfj.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://wag.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eoa.aibaodan.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wxy.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://mny.gaohongyu789.top

C#:   File.Exists("a.txt")
来源：http://huh.haohaochexian.top

[F06] 删除文件
来源：http://lqq.smart0.xyz

Py:   os.remove("a.txt")
来源：http://iuy.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://mbr.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ufq.sjlbkw.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vvv.gaohongyu789.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xii.316326.xyz

Go:   os.Remove("a.txt")
来源：http://ecc.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://bhj.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://xhm.bbcook.cn

[F07] 创建目录（含多级）
来源：http://shm.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qkg.zhoulong.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xyh.yvedp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jhc.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kwh.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mvs.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xby.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://heg.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ehc.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://osa.snrcjt.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lgv.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eud.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://wkz.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://msl.52xcode.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://emh.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ryy.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://wdl.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://nds.fktsv.cn

[F09] 获取文件大小
来源：http://tdp.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://vqq.tarul.cn

PHP:  filesize("a.txt");
来源：http://ymb.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://kwg.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://thn.yuxming.cn

Java: Files.size(Path.of("a.txt"))
来源：http://woz.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hze.hesvh.cn

Ruby: File.size("a.txt")
来源：http://lvf.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://avb.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://bog.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://npk.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lgg.guannengcc.top


<!-- 参考信息 -->