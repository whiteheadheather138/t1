代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://czo.gzhubu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tym.svipenyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cdo.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bih.vehdjk.com

[E02] 重复字符串
来源：http://tkf.wangshuangyany.cn

Py:   "ab" * 3
来源：http://uua.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://zkc.mhx1999.top

JS:   "ab".repeat(3)
来源：http://xrw.uphjek.com

TS:   "ab".repeat(3)
来源：http://dpc.dashuyun.cn

Java: "ab".repeat(3)
来源：http://zpz.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://csr.wangdashe.top

Ruby: "ab" * 3
来源：http://ufu.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://doa.pycfn.com

[E03] 截取子串
来源：http://bhx.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ysw.hysaishi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bnk.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cbb.epnwcf.com

TS:   s.slice(1, 4)
来源：http://pmp.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://dru.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vfx.yj20258.top

Ruby: s[1, 3];  s[1..3]
来源：http://cqi.jqgfzy.top

C#:   s.Substring(1, 3)
来源：http://nrk.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://htr.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://doe.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://yyp.cheryme.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mzh.pycfn.com

TS:   s.indexOf("x")
来源：http://cko.yongpay.top

Java: s.indexOf("x")
来源：http://ljs.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://zlx.fengsongda.top

Ruby: s.index("x")
来源：http://oxy.jqgfzy.top

C#:   s.IndexOf("x")
来源：http://nht.hysaishi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lnt.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lxo.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vnt.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ayf.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wwq.jianghu66.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zbo.daria6918.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ipi.fktsv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lzu.yj20258.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ibk.cucudq.cn

[E06] 替换子串
来源：http://zld.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://chg.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://bvh.gzhubu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fbl.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://eum.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oss.yanxiufei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ukl.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dnh.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://ovu.gzhubu.top

[E07] 按分隔符拆分
来源：http://nya.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hjv.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uzw.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fwj.svipenyu.cn

TS:   s.split(",")
来源：http://yfa.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gmg.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ypj.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://phx.sjlbkw.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://twr.hywenlv.cn

[E08] 数组按分隔符合并
来源：http://soj.jianghu66.top

Py:   ",".join(items)
来源：http://eay.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://jtk.feifeiyinyue.top

JS:   items.join(",")
来源：http://hfw.hfpthk.cn

TS:   items.join(",")
来源：http://pio.ybcxt.top

Java: String.join(",", items)
来源：http://duq.meibo888.top

Go:   strings.Join(items, ",")
来源：http://uvg.yj20258888.top

Ruby: items.join(",")
来源：http://yfp.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://bgk.ivvv.top

[E09] 去除所有空白字符
来源：http://pof.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rrt.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fcg.bjfxy.top

JS:   s.replace(/\s+/g, "")
来源：http://jya.cashguo.top

TS:   s.replace(/\s+/g, "")
来源：http://zin.yfazqb.com

Java: s.replaceAll("\\s+", "")
来源：http://psx.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vao.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://zue.yonumen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ail.guannengcc.top

[E10] 左侧补零 / 定长填充
来源：http://ltf.nanxuanxn.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nbd.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hiy.nanxinkj.top

JS:   "7".padStart(3, "0")
来源：http://tbe.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://jdn.xinyue.icu

Java: String.format("%03d", 7)
来源：http://cvs.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lll.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fpg.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fjt.ehwqpu.com

[E11] 反转字符串
来源：http://bzk.jinqigfzy.top

Py:   s[::-1]
来源：http://vsb.zdqjudy.top

PHP:  strrev($s);
来源：http://dmk.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://vqk.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://czs.uphjek.com

Java: new StringBuilder(s).reverse().toString()
来源：http://uxx.nwbrower.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bmw.wangshuangyany.cn

Ruby: s.reverse
来源：http://yyl.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://ita.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://rxr.ivvv.top

Py:   s.count("a")
来源：http://ofg.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://skk.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://bsp.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://zpb.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lgl.dashuyun.cn

Go:   strings.Count(s, "a")
来源：http://jko.ydjk.org.cn

Ruby: s.count("a")
来源：http://jfq.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://tyj.shanyushiyangkeji.top

[E13] 逐字符遍历
来源：http://swe.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://uut.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qmc.zhengqikj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lxe.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://qfu.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vlz.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ake.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lwx.cashguo.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aat.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://zjg.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://crz.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://iej.jinqigufen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://err.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://szz.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uxx.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gdd.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vom.hammf.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gun.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://szj.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kps.ywan-chungtsiang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nlg.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kxu.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mer.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eix.sweek.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bhh.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mwk.gzhubu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fen.zhongyouzk.top

[E16] 数字千分位
来源：http://lhc.yj202588.top

Py:   f"{1234567:,}"
来源：http://wua.hesvh.cn

PHP:  number_format(1234567);
来源：http://uat.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vxi.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://uem.fktsv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dar.yj20258888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xyu.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gfu.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://wfu.cdnleiting.top

[E17] 首字母大写
来源：http://fwd.kuanghao11.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ysv.tianlin.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://hyb.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jjf.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://api.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sik.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://crq.wangdashe.top

Ruby: s.capitalize
来源：http://wjt.zycfv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pcw.bbcook.cn

[E18] 模板占位符替换
来源：http://yqe.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kbp.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fkc.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bbf.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lyb.ydzc1.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ghe.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zxd.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zst.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xyo.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://mpo.yfazqb.com

Py:   s.splitlines()
来源：http://vtq.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wrq.ivvv.top

JS:   s.split(/\r?\n/)
来源：http://kxm.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://scb.yfazqb.com

Java: s.lines().toList()
来源：http://jqm.jinqigufen.top

Go:   strings.Split(s, "\n")
来源：http://eru.hfpthk.cn

Ruby: s.lines
来源：http://lph.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://yci.sweek.top

[E20] 判断字符串是否为空
来源：http://sxn.ybcxt.top

Py:   if not s:
来源：http://yqb.tarul.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vvo.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xde.hnxiangtu.top

TS:   if (s === "") {}
来源：http://igr.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://tjo.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://luv.tianlin.xyz

Ruby: if s.empty?
来源：http://ezb.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vzp.smart0.xyz

[E21] 超长截断加省略号
来源：http://xrb.shuidangran.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mag.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qhi.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fxn.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bct.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eti.zhijiandao.cn

Go:   // 按 rune 判断长度后截断
来源：http://eae.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://huj.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xcz.xinyue.icu

[E22] 字节长度与字符长度
来源：http://ezp.cheryme.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wor.ydjk.org.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dzb.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://otz.feifeiyinyue.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ocl.yueranfly.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cxr.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bqi.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://xtq.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xuq.nanxuanxn.top

================================================================================
来源：http://fwj.ydzc1.top

F. 文件与目录
来源：http://tcl.yangfankeji.com

================================================================================
来源：http://mwk.xuetiantiany.cn

[F01] 读取整个文件
来源：http://ena.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ber.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://xky.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xwn.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://csv.9152youxi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mnk.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mbj.bjfxy.top

Ruby: File.read("a.txt")
来源：http://iru.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://esi.shzxlz.cn

[F02] 逐行读取文件
来源：http://pvl.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qvm.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gku.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mea.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yqa.ehwqpu.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ett.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ukl.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xeu.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wzb.dianchejie.cn

[F03] 写入文件（覆盖）
来源：http://jxq.birdmap.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ygz.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sqz.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eeq.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://umg.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hup.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pvr.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://xgf.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tkb.ivvv.top

[F04] 追加写入文件
来源：http://oli.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://akh.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bav.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cfl.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://say.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vrm.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ypq.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fti.hongshengwenyu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rhc.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://und.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hzc.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://dfx.zhijiandao.cn

JS:   fs.existsSync("a.txt")
来源：http://wcg.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://wqb.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://rif.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://maq.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://ocm.ivvv.top

C#:   File.Exists("a.txt")
来源：http://snd.zhiwuduotai.top

[F06] 删除文件
来源：http://uzs.tarul.cn

Py:   os.remove("a.txt")
来源：http://ban.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://lce.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://emn.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://ifs.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://spv.pycfn.com

Go:   os.Remove("a.txt")
来源：http://unq.hammf.cn

Ruby: File.delete("a.txt")
来源：http://fuv.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://rho.nwbrower.top

[F07] 创建目录（含多级）
来源：http://ulz.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wpz.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uft.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://soz.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ldc.gaohongyu789.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bpn.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ajm.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aaw.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tei.smart0.xyz

[F08] 遍历目录
来源：http://xte.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tvz.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xmx.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://mdm.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://rnr.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tnr.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yhd.vehdjk.com

Ruby: Dir.children("dir")
来源：http://ryf.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://yxi.ydzc1.top

[F09] 获取文件大小
来源：http://psx.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://gmx.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://hom.ehwqpu.com

JS:   fs.statSync("a.txt").size
来源：http://huf.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://msm.gaohongyu789.top

Java: Files.size(Path.of("a.txt"))
来源：http://jxk.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rre.bjfxy.top

Ruby: File.size("a.txt")
来源：http://qmj.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://quv.zhixingplan.top

[F10] 取文件扩展名 / 文件名
来源：http://xej.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xqi.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mpj.hnqzz.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mub.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://dzx.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jdv.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fxm.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gix.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qko.zdbjq.cn

[F11] 复制与移动文件
来源：http://nxk.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fmh.gaohongyu789.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ome.yfazqb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cae.hywenlv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://efm.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mxy.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zkm.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oid.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ygn.jqgfzy.top

[F12] CSV 读写
来源：http://csr.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rif.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qkz.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jye.dianchejie.cn

TS:   // 同上
来源：http://jod.zdbjq.cn


<!-- 参考信息 -->