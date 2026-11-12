代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hno.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pee.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yly.xylfe.cn

[D26] 数组转字符串
来源：http://rie.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://hdo.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://ksu.vehdjk.com

JS:   arr.join(", ")
来源：http://drc.ydjk.org.cn

TS:   arr.join(", ")
来源：http://roz.yongpay.top

Java: String.join(", ", list)
来源：http://lqd.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://kwb.jianghu66.top

Ruby: arr.join(", ")
来源：http://avx.xinyue.icu

C#:   string.Join(", ", list)
来源：http://bam.0kj1m.cn

================================================================================
来源：http://yxq.316326.xyz

E. 字符串处理
来源：http://yqr.cdnleiting.top

================================================================================
来源：http://wlr.yueranfly.top

[E01] 拼接字符串
来源：http://axq.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yhf.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fgn.ctjpmb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zlw.yuxming.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pue.ydjk.org.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ync.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zhq.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://moz.uphjek.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yze.snrcjt.cn

[E02] 重复字符串
来源：http://nna.gzhubu.top

Py:   "ab" * 3
来源：http://aiw.ctjpmb.com

PHP:  str_repeat("ab", 3);
来源：http://lmy.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://olu.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://cih.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://tep.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://bss.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://ieh.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fbt.iojbl.cn

[E03] 截取子串
来源：http://ikf.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://omo.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rws.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://otb.sjlbkw.cn

TS:   s.slice(1, 4)
来源：http://eej.aizwys.cn

Java: s.substring(1, 4)
来源：http://vfg.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://udv.bjfxy.top

Ruby: s[1, 3];  s[1..3]
来源：http://ewp.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://jmd.jianghu66.top

[E04] 查找子串位置
来源：http://cvn.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://zxk.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://tql.pycfn.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kox.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://zxu.daxiang520.top

Java: s.indexOf("x")
来源：http://iym.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://yrf.316326.xyz

Ruby: s.index("x")
来源：http://hio.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://vwk.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://obr.havefunace.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ucq.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ksg.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kii.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ukl.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tbv.ydjk.org.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jpo.sysykeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nxf.quarkkingdee.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hda.hcnkem.com

[E06] 替换子串
来源：http://bjp.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dia.kuanghao11.cn

PHP:  str_replace("a", "b", $s);
来源：http://fmk.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xod.guowangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://smc.zhongyouzk.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yfu.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oyg.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nmq.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://stu.epnwcf.com

[E07] 按分隔符拆分
来源：http://lkj.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jzv.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jwn.jinghuilouyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cmx.xziqi.cn

TS:   s.split(",")
来源：http://hjq.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mcm.nanxuanxn.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lzo.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://fhk.9152youxi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zev.hnqzz.top

[E08] 数组按分隔符合并
来源：http://lzs.c1oappe.top

Py:   ",".join(items)
来源：http://naq.epnwcf.com

PHP:  implode(",", $items);
来源：http://wlm.yuanzhike.top

JS:   items.join(",")
来源：http://vom.yongpay.top

TS:   items.join(",")
来源：http://pic.zhijiandao.cn

Java: String.join(",", items)
来源：http://iiw.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://liz.vqdsnc.cn

Ruby: items.join(",")
来源：http://eut.52xcode.cn

C#:   string.Join(",", items)
来源：http://nep.hysaishi.cn

[E09] 去除所有空白字符
来源：http://ntc.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pro.feifeiyinyue.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eia.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://shg.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://cev.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://qry.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://biv.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://axi.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gss.fktsv.cn

[E10] 左侧补零 / 定长填充
来源：http://muh.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lpn.zhiwuduotai.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oeb.shangyingyoupin.top

JS:   "7".padStart(3, "0")
来源：http://iwj.yonumen.top

TS:   "7".padStart(3, "0")
来源：http://pid.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://ngb.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fcv.zhoulong.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dgi.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://luw.yuanzhike.top

[E11] 反转字符串
来源：http://hnv.yuxming.cn

Py:   s[::-1]
来源：http://zgb.zdbjq.cn

PHP:  strrev($s);
来源：http://fdi.daxiang520.top

JS:   [...s].reverse().join("")
来源：http://iqs.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://sno.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://rsn.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://agg.bjfxy.top

Ruby: s.reverse
来源：http://lov.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://kja.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://wya.cucudq.cn

Py:   s.count("a")
来源：http://nka.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://kfg.jinghuilouyu.cn

JS:   s.split("a").length - 1
来源：http://oku.xziqi.cn

TS:   s.split("a").length - 1
来源：http://yis.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://epr.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://sbk.wangshuangyany.cn

Ruby: s.count("a")
来源：http://ggl.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://oxx.shzxlz.cn

[E13] 逐字符遍历
来源：http://kxo.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://evc.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nwc.shuidangran.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qrw.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ere.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fcg.ehwqpu.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://efa.zycfv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kyr.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qzk.52xcode.cn

[E14] URL 编码与 Base64
来源：http://ygr.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://onj.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jpb.chenzaomai.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hly.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fxe.feifeiyinyue.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tze.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qij.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nhu.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://igj.andypj.xyz

[E15] HTML 转义 / 反转义
来源：http://kob.kuanghao11.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zxp.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://slu.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fbb.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://jtk.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ekn.ivvv.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zsz.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iml.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sqd.meibo888.top

[E16] 数字千分位
来源：http://nbk.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://uil.sxryk.cn

PHP:  number_format(1234567);
来源：http://pdm.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jck.zdbjq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wzn.gogol.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tex.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pag.ctjpmb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ssa.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://lml.316326.xyz

[E17] 首字母大写
来源：http://evu.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://elk.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://fmr.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ikj.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fsi.daxiang520.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ilg.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://csr.redwolf501.top

Ruby: s.capitalize
来源：http://uzn.yangfankeji.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://njs.xuanzx.com

[E18] 模板占位符替换
来源：http://esm.jyoumei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://itb.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dbq.ctjpmb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://eus.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gdd.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fei.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wsy.yongpay.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vrc.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mtc.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://kzf.fktsv.cn

Py:   s.splitlines()
来源：http://aze.ydzc1.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ncb.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://lul.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://xdw.yj20258.top

Java: s.lines().toList()
来源：http://khu.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://fsn.bjfxy.top

Ruby: s.lines
来源：http://qfg.hfpthk.cn

C#:   s.Split('\n')
来源：http://kdd.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://beu.fzhhl.top

Py:   if not s:
来源：http://mpy.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xzw.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qat.jinqigfzy.top

TS:   if (s === "") {}
来源：http://amy.hnxiangtu.top

Java: if (s.isEmpty()) {}
来源：http://bgb.andypj.xyz

Go:   if s == "" {}
来源：http://lrt.dashuyun.cn

Ruby: if s.empty?
来源：http://ieh.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qtv.yj202588.top

[E21] 超长截断加省略号
来源：http://czm.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fvs.xziqi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ugm.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tpz.shuidangran.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vph.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bbr.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://ctz.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lkl.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://msx.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://hpf.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ocx.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aqq.xuanzx.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hge.dianchejie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pkj.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hkp.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jfo.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://vvn.sjlbkw.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qgf.hnqzz.top

================================================================================
来源：http://iyr.hesvh.cn

F. 文件与目录
来源：http://ddy.yueranfly.top

================================================================================
来源：http://afi.redwolf501.top

[F01] 读取整个文件
来源：http://qfz.daria6918.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nsv.jianghu66.top

PHP:  file_get_contents("a.txt");
来源：http://own.ivvv.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mew.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pji.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://evm.yuxming.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://psc.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://hdo.dashuyun.cn

C#:   File.ReadAllText("a.txt");
来源：http://dgb.nanxuanxn.top

[F02] 逐行读取文件
来源：http://jws.pengpengdd.cyou

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tey.tianlin.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://luc.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eam.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pnk.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://giy.ivvv.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mqy.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zbp.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vpi.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://nko.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://avm.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dmp.epnwcf.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://obb.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ztu.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pxr.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eyv.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://zsd.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nnr.jyoumei.cn

[F04] 追加写入文件
来源：http://kwz.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sop.fengsongda.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lya.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://huf.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nqa.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hli.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jhq.zycfv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mmj.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://djt.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://kwn.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mdi.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://bge.fktsv.cn

JS:   fs.existsSync("a.txt")
来源：http://dty.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://gtw.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eoe.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gzf.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://nai.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://bgd.yvedp.cn

[F06] 删除文件
来源：http://mlc.xinyue.icu

Py:   os.remove("a.txt")
来源：http://uqw.meibo888.top

PHP:  unlink("a.txt");
来源：http://yzu.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://hlp.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://zzq.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ovi.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://rjs.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://gzj.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://tzr.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://wih.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dso.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tol.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iui.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yos.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aqj.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wrw.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pia.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wce.hnqzz.top

[F08] 遍历目录
来源：http://xgr.c1oappe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xnf.zhengqikj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iok.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://kcy.shuidangran.top

TS:   fs.readdirSync("dir")
来源：http://ibq.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tdn.hnqzz.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sno.sweek.top

Ruby: Dir.children("dir")
来源：http://aix.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://ayv.ctjpmb.com

[F09] 获取文件大小
来源：http://uyd.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://tjk.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://wpq.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://nil.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://yct.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://ckx.yangfankeji.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dvn.wangdashe.top

Ruby: File.size("a.txt")
来源：http://sld.yfazqb.com

C#:   new FileInfo("a.txt").Length
来源：http://ipq.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://whi.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gki.ppjwa.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zcy.ydjk.org.cn


<!-- 参考信息 -->