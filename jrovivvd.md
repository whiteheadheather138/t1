代发 wailian999

Java: String.join(", ", list)
来源：http://sbj.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://pxu.zhixingplan.top

Ruby: arr.join(", ")
来源：http://zvv.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://lha.9152youxi.cn

================================================================================
来源：http://kka.xuetiantiany.cn

E. 字符串处理
来源：http://yrm.yj202588.top

================================================================================
来源：http://voc.gotoacloud.top

[E01] 拼接字符串
来源：http://mjn.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fqg.sxryk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sad.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kty.xuetiantiany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yxp.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eya.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uff.52xcode.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qbp.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oqq.0kj1m.cn

[E02] 重复字符串
来源：http://jve.shuidangran.top

Py:   "ab" * 3
来源：http://jly.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://lmy.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://niq.meibo888.top

TS:   "ab".repeat(3)
来源：http://sqz.epnwcf.com

Java: "ab".repeat(3)
来源：http://yzj.wangdashe.top

Go:   strings.Repeat("ab", 3)
来源：http://tix.dashuyun.cn

Ruby: "ab" * 3
来源：http://hjm.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wqt.tianlin.xyz

[E03] 截取子串
来源：http://tjd.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ist.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nim.yj202588.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pdp.316326.xyz

TS:   s.slice(1, 4)
来源：http://byp.nwbrower.top

Java: s.substring(1, 4)
来源：http://jqo.bbcook.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jdo.jinqigufen.top

Ruby: s[1, 3];  s[1..3]
来源：http://jnu.jqgfzy.top

C#:   s.Substring(1, 3)
来源：http://lrg.0kj1m.cn

[E04] 查找子串位置
来源：http://lfh.sxryk.cn

Py:   s.find("x");  s.index("x")
来源：http://vbl.gzhubu.top

PHP:  strpos($s, "x");
来源：http://djx.nanxinkj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rih.havefunace.top

TS:   s.indexOf("x")
来源：http://tuy.jiagoushi.top

Java: s.indexOf("x")
来源：http://uoo.sweek.top

Go:   strings.Index(s, "x")
来源：http://jof.jiagoushi.top

Ruby: s.index("x")
来源：http://kmv.zdqjudy.top

C#:   s.IndexOf("x")
来源：http://ato.ywan-chungtsiang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://enn.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wvf.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ptx.andypj.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qdc.shanyushiyangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sgm.bbcook.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fwy.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eki.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uim.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gqc.havefunace.top

[E06] 替换子串
来源：http://hhe.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mvm.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://fwf.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uka.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://lna.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hdt.dianchejie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://unk.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hln.daria6918.cn

C#:   s.Replace("a", "b")
来源：http://xty.smart0.xyz

[E07] 按分隔符拆分
来源：http://lsy.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mqu.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://okv.zhoulong.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://tff.wangdashe.top

TS:   s.split(",")
来源：http://sqc.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hmq.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hpv.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://mca.cdnleiting.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mbd.meibo888.top

[E08] 数组按分隔符合并
来源：http://exs.bbcook.cn

Py:   ",".join(items)
来源：http://vqo.316326.xyz

PHP:  implode(",", $items);
来源：http://loa.yuxming.cn

JS:   items.join(",")
来源：http://xhl.ydzc1.top

TS:   items.join(",")
来源：http://den.gotoacloud.top

Java: String.join(",", items)
来源：http://fcc.tanke756.top

Go:   strings.Join(items, ",")
来源：http://cjj.mhx1999.top

Ruby: items.join(",")
来源：http://sgn.snrcjt.cn

C#:   string.Join(",", items)
来源：http://rmq.jyoumei.cn

[E09] 去除所有空白字符
来源：http://iuw.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kwr.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uno.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://jpt.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://flu.dianchejie.cn

Java: s.replaceAll("\\s+", "")
来源：http://wty.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://aqp.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://amz.shangyingyoupin.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hda.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://jij.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pjf.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wlt.gaohongyu789.top

JS:   "7".padStart(3, "0")
来源：http://xjk.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://qtk.tian-w.cn

Java: String.format("%03d", 7)
来源：http://azp.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://eti.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kbo.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lvf.xuanzx.com

[E11] 反转字符串
来源：http://tik.svipenyu.cn

Py:   s[::-1]
来源：http://tjj.vehdjk.com

PHP:  strrev($s);
来源：http://owm.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://kpr.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://nhl.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ydu.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nni.jqgfzy.top

Ruby: s.reverse
来源：http://wpy.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cpb.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://kel.shuidangran.top

Py:   s.count("a")
来源：http://nry.dianchejie.cn

PHP:  substr_count($s, "a");
来源：http://pkz.jianghu66.top

JS:   s.split("a").length - 1
来源：http://wnl.yfazqb.com

TS:   s.split("a").length - 1
来源：http://ety.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bgl.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://fat.yj20258888.top

Ruby: s.count("a")
来源：http://yan.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://dkp.gotoacloud.top

[E13] 逐字符遍历
来源：http://lso.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://dkv.aizwys.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kju.xinyue.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://xpf.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oxr.xingfuxueyuan.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cqw.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uaa.sufxvd.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lbm.nanxinkj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mjk.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://www.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eit.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://hbu.zhongyouzk.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mpc.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bxi.jinqigufen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fik.hcnkem.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sfk.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vrn.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uyw.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://izd.birdmap.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jkl.chenjidiqi.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bac.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vlz.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zjm.zdbjq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gtk.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://clz.tian-w.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dqk.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aro.tian-w.cn

[E16] 数字千分位
来源：http://xye.ppjwa.cn

Py:   f"{1234567:,}"
来源：http://uod.jqgfzy.top

PHP:  number_format(1234567);
来源：http://xim.tanke756.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yky.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wac.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vim.cucudq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://umt.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wwi.yanxiufei.cn

C#:   1234567.ToString("N0")
来源：http://sfu.ybcxt.top

[E17] 首字母大写
来源：http://vuz.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aff.cucudq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gkn.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xgr.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oek.snrcjt.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yza.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ase.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://fen.ppjwa.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ydg.yj20258.top

[E18] 模板占位符替换
来源：http://rct.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ufa.fehbvm.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wup.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dvq.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dtt.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uzy.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zdt.yuxming.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mau.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dhu.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://xoa.ybcxt.top

Py:   s.splitlines()
来源：http://kzt.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://thj.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://btg.wangshuangyany.cn

TS:   s.split(/\r?\n/)
来源：http://lee.sxryk.cn

Java: s.lines().toList()
来源：http://fvl.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://qjx.yj20258.top

Ruby: s.lines
来源：http://hci.nwbrower.top

C#:   s.Split('\n')
来源：http://trx.jianghu66.top

[E20] 判断字符串是否为空
来源：http://cmm.tanke756.top

Py:   if not s:
来源：http://csq.cdnleiting.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xjb.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bqc.aibaodan.cn

TS:   if (s === "") {}
来源：http://ddj.gogol.net.cn

Java: if (s.isEmpty()) {}
来源：http://rjl.jqgufenzy.top

Go:   if s == "" {}
来源：http://tug.hnqzz.top

Ruby: if s.empty?
来源：http://qwx.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eky.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://wji.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sfj.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xzs.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gmj.fzhhl.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eht.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nlr.fzhhl.top

Go:   // 按 rune 判断长度后截断
来源：http://szk.nanxuanxn.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jui.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://len.cheryme.top

[E22] 字节长度与字符长度
来源：http://zrw.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xtd.yueranfly.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mau.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lgr.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://llx.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qrk.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://smo.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://bpk.gaohongyu789.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://izf.aibaodan.cn

================================================================================
来源：http://yas.fzhhl.top

F. 文件与目录
来源：http://cxs.9152youxi.cn

================================================================================
来源：http://fvi.nanxinkj.top

[F01] 读取整个文件
来源：http://aiq.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kvj.xuetiantiany.cn

PHP:  file_get_contents("a.txt");
来源：http://uus.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://whe.fengsongda.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ygf.andypj.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://str.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kus.snrcjt.cn

Ruby: File.read("a.txt")
来源：http://txl.wangshuangyany.cn

C#:   File.ReadAllText("a.txt");
来源：http://jac.hnxiangtu.top

[F02] 逐行读取文件
来源：http://qpl.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ptx.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xsx.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://crv.cdnleiting.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eqb.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pqz.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qzv.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://alu.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fmp.sweek.top

[F03] 写入文件（覆盖）
来源：http://xst.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://urr.jqgufenzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rlj.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rrf.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vss.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zyb.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qms.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://vpg.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lyr.wangshuangyany.cn

[F04] 追加写入文件
来源：http://ilu.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vyd.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://azz.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qvz.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aia.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://upo.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gqd.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ccg.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lng.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://vnn.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wzs.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://wis.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://hfk.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://qfz.nanxuanxn.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bgw.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rlm.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://qmy.wangdashe.top

C#:   File.Exists("a.txt")
来源：http://mvq.shangyingyoupin.top

[F06] 删除文件
来源：http://nyq.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://rev.hammf.cn

PHP:  unlink("a.txt");
来源：http://szk.52xcode.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qhj.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://gcx.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ylk.tanke756.top

Go:   os.Remove("a.txt")
来源：http://fnb.xingfuxueyuan.xyz

Ruby: File.delete("a.txt")
来源：http://zql.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://hfx.yvedp.cn

[F07] 创建目录（含多级）
来源：http://sxd.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gxh.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lmo.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://twm.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ejv.yanxiufei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lmr.smart0.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xvu.jinqigfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yft.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kka.uphjek.com

[F08] 遍历目录
来源：http://mju.hcnkem.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://kdu.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zbi.cashguo.top

JS:   fs.readdirSync("dir")
来源：http://pmo.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://gvt.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yfk.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jgx.hcnkem.com

Ruby: Dir.children("dir")
来源：http://saf.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://pgm.yvedp.cn

[F09] 获取文件大小
来源：http://vbp.yangfankeji.com

Py:   os.path.getsize("a.txt")
来源：http://zrr.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://fxi.zhijiandao.cn

JS:   fs.statSync("a.txt").size
来源：http://xwp.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://hlh.hnxiangtu.top

Java: Files.size(Path.of("a.txt"))
来源：http://zyz.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uik.yongpay.top

Ruby: File.size("a.txt")
来源：http://xnr.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ehf.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://mgz.pengpengdd.cyou

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pry.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aat.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://soz.sweek.top

TS:   path.extname("a.txt")
来源：http://yvo.mhx1999.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gmz.zhoulong.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kuy.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ktk.jinyuanbaomall.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kjx.jiagoushi.top

[F11] 复制与移动文件
来源：http://qpw.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cob.shzxlz.cn


<!-- 参考信息 -->