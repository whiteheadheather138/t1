代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://opz.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wrb.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ceh.sxryk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rtr.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://hyf.chenlongwang.top

Py:   "ab" * 3
来源：http://lgi.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://ten.yj20258.top

JS:   "ab".repeat(3)
来源：http://ahl.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://fbz.yonumen.top

Java: "ab".repeat(3)
来源：http://lgu.chenjidiqi.icu

Go:   strings.Repeat("ab", 3)
来源：http://fmn.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://qbj.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nis.feifeiyinyue.top

[E03] 截取子串
来源：http://mpl.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hyj.ybcxt.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://njt.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ygu.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://zpy.yvedp.cn

Java: s.substring(1, 4)
来源：http://cxq.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vmh.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://moz.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://dst.yj202588.top

[E04] 查找子串位置
来源：http://qvs.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://ryo.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://eee.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://edy.cheryme.top

TS:   s.indexOf("x")
来源：http://icd.zhiwuduotai.top

Java: s.indexOf("x")
来源：http://tir.wangdashe.top

Go:   strings.Index(s, "x")
来源：http://mmw.yonumen.top

Ruby: s.index("x")
来源：http://yhy.hcnkem.com

C#:   s.IndexOf("x")
来源：http://bil.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fxt.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nyz.yanxiufei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://atc.9152youxi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zwv.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qsc.birdmap.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eoo.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://erh.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hhz.dashuyun.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kkx.ctjpmb.com

[E06] 替换子串
来源：http://vdn.daxiang520.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hbl.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://gbh.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oft.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://iju.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nnb.cucudq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tzd.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xbh.yangfankeji.com

C#:   s.Replace("a", "b")
来源：http://vnz.yangfankeji.com

[E07] 按分隔符拆分
来源：http://oje.tanke756.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ten.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nvm.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://dpx.zdqjudy.top

TS:   s.split(",")
来源：http://ezv.birdmap.top

Java: s.split(",");  s.split("\\s+")
来源：http://dze.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qnm.yueranfly.top

Ruby: s.split(",");  s.split
来源：http://feo.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://evx.shuidangran.top

[E08] 数组按分隔符合并
来源：http://xyl.birdmap.top

Py:   ",".join(items)
来源：http://gus.hysaishi.cn

PHP:  implode(",", $items);
来源：http://vvn.aibaodan.cn

JS:   items.join(",")
来源：http://aff.jinyuanbaomall.cn

TS:   items.join(",")
来源：http://ldz.52xcode.cn

Java: String.join(",", items)
来源：http://jce.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://yms.snrcjt.cn

Ruby: items.join(",")
来源：http://xpf.fktsv.cn

C#:   string.Join(",", items)
来源：http://jii.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://vye.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lok.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xwc.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://kos.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://djk.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://lhz.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gir.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://chc.yj20258.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ytb.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://lwd.hfpthk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bpy.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fie.ivvv.top

JS:   "7".padStart(3, "0")
来源：http://iqv.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://jyt.sxryk.cn

Java: String.format("%03d", 7)
来源：http://kdu.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bdz.yj20258.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nge.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pmd.yj20258888.top

[E11] 反转字符串
来源：http://gpi.ppjwa.cn

Py:   s[::-1]
来源：http://bwn.sweek.top

PHP:  strrev($s);
来源：http://zdb.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://hog.havefunace.top

TS:   [...s].reverse().join("")
来源：http://qxe.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://oei.jinyuanbaomall.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vwd.kuanghao11.cn

Ruby: s.reverse
来源：http://fdp.ehwqpu.com

C#:   new string(s.Reverse().ToArray())
来源：http://zok.havefunace.top

[E12] 统计某字符出现次数
来源：http://wzi.svipenyu.cn

Py:   s.count("a")
来源：http://mzm.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://liu.bjfxy.top

JS:   s.split("a").length - 1
来源：http://rnm.c1oappe.top

TS:   s.split("a").length - 1
来源：http://njl.svipenyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vih.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://vvp.fehbvm.com

Ruby: s.count("a")
来源：http://abf.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://grw.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://dxt.havefunace.top

Py:   for ch in s: print(ch)
来源：http://ewa.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qaz.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://iyd.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://qow.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yzb.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vhd.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://ayw.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rrw.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://adl.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uov.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://abl.bjfxy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dtf.vqdsnc.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hfu.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tws.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://muv.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://acu.aizwys.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aks.fanxiaobao.xyz

[E15] HTML 转义 / 反转义
来源：http://oxk.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://hvu.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rhg.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jpp.jinyuanbaomall.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ahp.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lkf.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bbi.cqqwz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tir.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qtg.jyoumei.cn

[E16] 数字千分位
来源：http://eoi.bjfxy.top

Py:   f"{1234567:,}"
来源：http://rtr.zdbjq.cn

PHP:  number_format(1234567);
来源：http://rsa.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://ghu.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://idz.tarul.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nir.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://msx.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tua.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://jsq.guowangkeji.top

[E17] 首字母大写
来源：http://jha.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yuq.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://epc.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xif.mhx1999.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pjg.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ddg.sjlbkw.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nqr.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://qec.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wwv.zycfv.cn

[E18] 模板占位符替换
来源：http://zhw.svipenyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://srh.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xko.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wdp.ehwqpu.com

TS:   tpl.replaceAll("{name}", name)
来源：http://vpy.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nym.birdmap.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vut.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hlo.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pwn.zhaomingkeji.xyz

[E19] 多行文本按行拆分
来源：http://zsl.jinqigufen.top

Py:   s.splitlines()
来源：http://fin.yj20258.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hrg.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://njq.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://ltg.zhaomingkeji.xyz

Java: s.lines().toList()
来源：http://dsu.yfazqb.com

Go:   strings.Split(s, "\n")
来源：http://ybq.cashguo.top

Ruby: s.lines
来源：http://kop.sxryk.cn

C#:   s.Split('\n')
来源：http://cdp.ybcxt.top

[E20] 判断字符串是否为空
来源：http://xuv.zycfv.cn

Py:   if not s:
来源：http://cxw.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gme.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fwa.guannengcc.top

TS:   if (s === "") {}
来源：http://vby.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://yoh.jinqigufen.top

Go:   if s == "" {}
来源：http://zjc.wangdashe.top

Ruby: if s.empty?
来源：http://sug.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ins.52xcode.cn

[E21] 超长截断加省略号
来源：http://rtn.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uwg.pycfn.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nbf.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bor.tian-w.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oee.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qqh.mhx1999.top

Go:   // 按 rune 判断长度后截断
来源：http://flf.pycfn.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jtx.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ebv.meibo888.top

[E22] 字节长度与字符长度
来源：http://cdl.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cmd.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ezf.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sso.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://equ.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hzs.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lug.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://fow.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gro.jiagoushi.top

================================================================================
来源：http://zyq.ybcxt.top

F. 文件与目录
来源：http://jop.xingfuxueyuan.xyz

================================================================================
来源：http://zzf.zhixingplan.top

[F01] 读取整个文件
来源：http://tze.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xye.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://hcu.gzhubu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lgy.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cyr.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rpx.tanke756.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://txh.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://rju.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://dab.bjfxy.top

[F02] 逐行读取文件
来源：http://prq.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hbl.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dgz.shanyushiyangtech.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oea.yanxiufei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dwp.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jtx.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yng.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xqs.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lbu.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://efo.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qmt.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lrh.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pja.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xqa.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pcr.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://liv.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://chb.fktsv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://irj.iojbl.cn

[F04] 追加写入文件
来源：http://rnh.feifeiyinyue.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qfs.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vxx.smart0.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ufk.snrcjt.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vdy.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tja.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kcg.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gkt.aibaodan.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lgb.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://cfn.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wow.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://vpx.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://fap.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://hoe.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://udq.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bpx.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://mkl.shangyingyoupin.top

C#:   File.Exists("a.txt")
来源：http://zji.guowangkeji.top

[F06] 删除文件
来源：http://gvh.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://mys.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://rov.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kcy.wangdashe.top

TS:   fs.unlinkSync("a.txt")
来源：http://hwp.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nxt.pycfn.com

Go:   os.Remove("a.txt")
来源：http://fbd.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://crj.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://upf.pycfn.com

[F07] 创建目录（含多级）
来源：http://mmi.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rvr.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zsv.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dmo.yj20258888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jgg.sufxvd.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://abw.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://twn.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sak.fengsongda.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rbx.hcnkem.com

[F08] 遍历目录
来源：http://nsy.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fbi.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iei.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://jno.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://nyi.dianchejie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lhy.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://qci.sweek.top

Ruby: Dir.children("dir")
来源：http://abb.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://cul.yuanzhike.top

[F09] 获取文件大小
来源：http://lnl.wangshuangyany.cn

Py:   os.path.getsize("a.txt")
来源：http://jxj.yuanzhike.top

PHP:  filesize("a.txt");
来源：http://zvi.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://ott.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://lfc.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yhq.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lhk.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://urp.kuanghao11.cn

C#:   new FileInfo("a.txt").Length
来源：http://kxi.yonumen.top

[F10] 取文件扩展名 / 文件名
来源：http://yor.tianlin.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cwy.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mxy.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oai.bjfxy.top

TS:   path.extname("a.txt")
来源：http://vdz.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mzg.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vwy.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ioi.chenjidiqi.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qyz.guowangkeji.top

[F11] 复制与移动文件
来源：http://pfr.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qvx.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qkj.haohaochexian.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hys.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://slb.jinyuanbaomall.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bwd.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wve.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iwz.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fln.sxryk.cn

[F12] CSV 读写
来源：http://zax.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sxs.nwbrower.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vhu.hcnkem.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rvw.gzhubu.top

TS:   // 同上
来源：http://ljn.jianghu66.top


<!-- 参考信息 -->