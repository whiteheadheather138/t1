代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://pio.zhiwuduotai.top

PHP:  implode(", ", $arr);
来源：http://ukt.sweek.top

JS:   arr.join(", ")
来源：http://cqz.zdbjq.cn

TS:   arr.join(", ")
来源：http://gcj.yvedp.cn

Java: String.join(", ", list)
来源：http://yqq.sxryk.cn

Go:   strings.Join(strs, ", ")
来源：http://bar.zdqjudy.top

Ruby: arr.join(", ")
来源：http://cxx.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://rvg.shanyushiyangkeji.top

================================================================================
来源：http://mco.nanxinkj.top

E. 字符串处理
来源：http://gym.ywan-chungtsiang.top

================================================================================
来源：http://qhp.feifeiyinyue.top

[E01] 拼接字符串
来源：http://aak.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zfz.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qxw.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aos.cqqwz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rqr.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ryt.wangshuangyany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ikf.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oqk.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nql.snrcjt.cn

[E02] 重复字符串
来源：http://bsk.ydjk.org.cn

Py:   "ab" * 3
来源：http://kqy.daxiang520.top

PHP:  str_repeat("ab", 3);
来源：http://gnq.daxiang520.top

JS:   "ab".repeat(3)
来源：http://dka.xziqi.cn

TS:   "ab".repeat(3)
来源：http://nal.shuidangran.top

Java: "ab".repeat(3)
来源：http://tgc.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://euw.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://wzq.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kqa.jianghu66.top

[E03] 截取子串
来源：http://fds.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xio.xingfuxueyuan.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iyd.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ayu.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://aog.sxryk.cn

Java: s.substring(1, 4)
来源：http://zkp.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iyl.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://gtl.birdmap.top

C#:   s.Substring(1, 3)
来源：http://sfz.zdbjq.cn

[E04] 查找子串位置
来源：http://eub.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://kgg.yj20258888.top

PHP:  strpos($s, "x");
来源：http://wcv.zdqjudy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vqo.chenjidiqi.icu

TS:   s.indexOf("x")
来源：http://uji.sweek.top

Java: s.indexOf("x")
来源：http://zcj.cheryme.top

Go:   strings.Index(s, "x")
来源：http://ghy.hammf.cn

Ruby: s.index("x")
来源：http://isk.tian-w.cn

C#:   s.IndexOf("x")
来源：http://cxi.svipenyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cnh.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ypi.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tdn.ppjwa.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gno.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xpt.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zzf.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ehr.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vdn.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yqu.pengpengdd.cyou

[E06] 替换子串
来源：http://iqe.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ihu.316326.xyz

PHP:  str_replace("a", "b", $s);
来源：http://qai.wangshuangyany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://egf.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://tis.jqgufenzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zsw.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nmn.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jrl.havefunace.top

C#:   s.Replace("a", "b")
来源：http://qfj.ywan-chungtsiang.top

[E07] 按分隔符拆分
来源：http://wep.guannengcc.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qni.yueranfly.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fkj.hammf.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hsx.ivvv.top

TS:   s.split(",")
来源：http://ljk.sjlbkw.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fix.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oge.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://knq.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fpl.uphjek.com

[E08] 数组按分隔符合并
来源：http://zvw.0kj1m.cn

Py:   ",".join(items)
来源：http://uvx.gzhubu.top

PHP:  implode(",", $items);
来源：http://irj.hywenlv.cn

JS:   items.join(",")
来源：http://ckz.hesvh.cn

TS:   items.join(",")
来源：http://ufk.tanke756.top

Java: String.join(",", items)
来源：http://zpa.chenlongwang.top

Go:   strings.Join(items, ",")
来源：http://bfx.redwolf501.top

Ruby: items.join(",")
来源：http://gqe.cheryme.top

C#:   string.Join(",", items)
来源：http://gjc.daxiang520.top

[E09] 去除所有空白字符
来源：http://pcm.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mhq.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://voj.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://qjw.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://ogh.zdqjudy.top

Java: s.replaceAll("\\s+", "")
来源：http://yhj.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qyz.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://reg.aibaodan.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://grh.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://lth.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ufv.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kku.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://ryb.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://dws.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://nyj.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mzl.hysaishi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://umy.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://auw.bbcook.cn

[E11] 反转字符串
来源：http://lcj.gaohongyu789.top

Py:   s[::-1]
来源：http://fus.pycfn.com

PHP:  strrev($s);
来源：http://cag.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://zgn.yonumen.top

TS:   [...s].reverse().join("")
来源：http://cqc.ehwqpu.com

Java: new StringBuilder(s).reverse().toString()
来源：http://cnu.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://bgm.nanxinkj.top

Ruby: s.reverse
来源：http://bjz.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://avt.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://zgs.tanke756.top

Py:   s.count("a")
来源：http://xkt.hongshengwenyu.top

PHP:  substr_count($s, "a");
来源：http://dyw.sysykeji.top

JS:   s.split("a").length - 1
来源：http://mdi.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://vak.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rvt.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://eze.hcnkem.com

Ruby: s.count("a")
来源：http://pnt.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://rjn.jqgfzy.top

[E13] 逐字符遍历
来源：http://kpk.epnwcf.com

Py:   for ch in s: print(ch)
来源：http://qcv.zhengqikj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kvq.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cly.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rei.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nxs.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cal.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://isp.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zzx.yongpay.top

[E14] URL 编码与 Base64
来源：http://byj.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://idl.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xsv.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mna.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lhl.hywenlv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vrt.ppjwa.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hvp.fehbvm.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qhc.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dze.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://hzx.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://uop.ywan-chungtsiang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dxf.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sda.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rap.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hrd.daria6918.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bqb.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fdi.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wea.andypj.xyz

[E16] 数字千分位
来源：http://ojc.sxryk.cn

Py:   f"{1234567:,}"
来源：http://xou.cashguo.top

PHP:  number_format(1234567);
来源：http://iwp.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rum.iojbl.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://adf.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jje.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cav.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fms.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://nab.smart0.xyz

[E17] 首字母大写
来源：http://jlu.9152youxi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cmr.aizwys.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lmi.quarkkingdee.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ctf.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mmp.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kzi.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fkw.svipenyu.cn

Ruby: s.capitalize
来源：http://kdw.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ztu.yuxming.cn

[E18] 模板占位符替换
来源：http://uqg.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yzj.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nqw.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vtd.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gta.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aum.nanxuanxn.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kes.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mke.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tvf.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://ijc.hywenlv.cn

Py:   s.splitlines()
来源：http://seo.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pkk.nwbrower.top

JS:   s.split(/\r?\n/)
来源：http://zhd.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://oat.c1oappe.top

Java: s.lines().toList()
来源：http://szk.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://wsm.yueranfly.top

Ruby: s.lines
来源：http://zyf.aizwys.cn

C#:   s.Split('\n')
来源：http://nlg.ybcxt.top

[E20] 判断字符串是否为空
来源：http://kta.cqqwz.cn

Py:   if not s:
来源：http://pmd.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aey.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bhc.jinqigfzy.top

TS:   if (s === "") {}
来源：http://dlb.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://iuc.fehbvm.com

Go:   if s == "" {}
来源：http://wgn.yuxming.cn

Ruby: if s.empty?
来源：http://abu.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dki.yueranfly.top

[E21] 超长截断加省略号
来源：http://wgj.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kwk.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://agy.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wao.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hmv.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gjh.fehbvm.com

Go:   // 按 rune 判断长度后截断
来源：http://rzt.pycfn.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jqp.ywan-chungtsiang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wkv.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://ipf.mhx1999.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tvr.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mog.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xfn.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ifj.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mtr.tian-w.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iag.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://wvz.316326.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tiy.chenlongwang.top

================================================================================
来源：http://gzb.jinqigufen.top

F. 文件与目录
来源：http://pwk.tanke756.top

================================================================================
来源：http://ouf.andypj.xyz

[F01] 读取整个文件
来源：http://lww.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://slg.ybcxt.top

PHP:  file_get_contents("a.txt");
来源：http://hab.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uqo.andypj.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ypl.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://dnj.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rpv.cashguo.top

Ruby: File.read("a.txt")
来源：http://jza.jinyuanbaomall.cn

C#:   File.ReadAllText("a.txt");
来源：http://pnd.guannengcc.top

[F02] 逐行读取文件
来源：http://uok.havefunace.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uqj.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zil.zhijiandao.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kyq.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dhz.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lli.aizwys.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mcp.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hmj.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vgn.xylfe.cn

[F03] 写入文件（覆盖）
来源：http://dia.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dlx.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mjv.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fxn.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://osm.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wqn.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hmi.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://aql.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ksb.jianghu66.top

[F04] 追加写入文件
来源：http://imq.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zlp.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sro.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xnj.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://brz.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tmy.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ted.jiagoushi.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jqw.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://npd.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://kew.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xjf.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://jhi.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://adq.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://qzt.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kol.pengpengdd.cyou

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://adr.ctjpmb.com

Ruby: File.exist?("a.txt")
来源：http://xfs.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://ufc.chenlongwang.top

[F06] 删除文件
来源：http://opw.hesvh.cn

Py:   os.remove("a.txt")
来源：http://ghw.zhengqikj.top

PHP:  unlink("a.txt");
来源：http://xfi.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://dvy.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://ggi.zhaomingkeji.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bzu.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://ymx.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://nop.tanke756.top

C#:   File.Delete("a.txt");
来源：http://rar.yj20258888.top

[F07] 创建目录（含多级）
来源：http://gdf.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ana.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cop.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zow.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://btp.fehbvm.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://srx.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wxr.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ify.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://elg.pycfn.com

[F08] 遍历目录
来源：http://dbu.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://oat.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ufa.hesvh.cn

JS:   fs.readdirSync("dir")
来源：http://wft.gzhubu.top

TS:   fs.readdirSync("dir")
来源：http://mne.guowangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tqz.tianlin.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://wik.shangyingyoupin.top

Ruby: Dir.children("dir")
来源：http://bny.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://fzv.aibaodan.cn

[F09] 获取文件大小
来源：http://rxy.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://uep.hesvh.cn

PHP:  filesize("a.txt");
来源：http://xxf.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://ynf.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://wry.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://cxk.epnwcf.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dsg.uphjek.com

Ruby: File.size("a.txt")
来源：http://wgo.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://axt.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://dtg.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aei.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wvx.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ick.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://jrk.bjfxy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://krb.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lim.zycfv.cn


<!-- 参考信息 -->