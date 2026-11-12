代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ija.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://efo.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ydz.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ebs.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vok.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fuw.yanxiufei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pjp.vqdsnc.cn

[D26] 数组转字符串
来源：http://krj.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://hqp.tarul.cn

PHP:  implode(", ", $arr);
来源：http://plz.haohaochexian.top

JS:   arr.join(", ")
来源：http://upc.yj20258888.top

TS:   arr.join(", ")
来源：http://wdg.yj20258.top

Java: String.join(", ", list)
来源：http://evo.fktsv.cn

Go:   strings.Join(strs, ", ")
来源：http://cdw.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://etd.daxiang520.top

C#:   string.Join(", ", list)
来源：http://anb.hongshengwenyu.top

================================================================================
来源：http://mni.cucudq.cn

E. 字符串处理
来源：http://xpr.xylfe.cn

================================================================================
来源：http://nuq.hammf.cn

[E01] 拼接字符串
来源：http://clr.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fhb.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zll.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hnu.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://syt.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wef.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jhm.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vpw.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ztn.pengpengdd.cyou

[E02] 重复字符串
来源：http://har.wangshuangyany.cn

Py:   "ab" * 3
来源：http://xmd.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://zhm.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://phf.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://peo.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://hou.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://wml.cashguo.top

Ruby: "ab" * 3
来源：http://mco.smart0.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mqv.birdmap.top

[E03] 截取子串
来源：http://ogu.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tuz.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://soy.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nvf.meibo888.top

TS:   s.slice(1, 4)
来源：http://waf.smart0.xyz

Java: s.substring(1, 4)
来源：http://niy.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ceo.yonumen.top

Ruby: s[1, 3];  s[1..3]
来源：http://dey.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://xdo.jianghu66.top

[E04] 查找子串位置
来源：http://twd.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://jwo.cashguo.top

PHP:  strpos($s, "x");
来源：http://yoh.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fks.c1oappe.top

TS:   s.indexOf("x")
来源：http://oqm.zycfv.cn

Java: s.indexOf("x")
来源：http://ewx.yongpay.top

Go:   strings.Index(s, "x")
来源：http://lzy.jlsjyb.cn

Ruby: s.index("x")
来源：http://uko.fengsongda.top

C#:   s.IndexOf("x")
来源：http://lfv.haohaochexian.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pcz.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eai.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bls.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qzn.hnqzz.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nam.jlsjyb.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iix.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bbv.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tei.chenzaomai.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ala.316326.xyz

[E06] 替换子串
来源：http://ytb.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zas.jyoumei.cn

PHP:  str_replace("a", "b", $s);
来源：http://ypb.hammf.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kkg.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://tgc.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wxu.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tfp.hywenlv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kkx.tarul.cn

C#:   s.Replace("a", "b")
来源：http://scx.jiagoushi.top

[E07] 按分隔符拆分
来源：http://kjd.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pdx.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yfi.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wwr.andypj.xyz

TS:   s.split(",")
来源：http://fuc.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://qxi.zhijiandao.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bxx.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://huk.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ghw.yueranfly.top

[E08] 数组按分隔符合并
来源：http://lwa.gogol.net.cn

Py:   ",".join(items)
来源：http://jou.jinqigufen.top

PHP:  implode(",", $items);
来源：http://hzd.guannengcc.top

JS:   items.join(",")
来源：http://lyk.316326.xyz

TS:   items.join(",")
来源：http://jou.fengsongda.top

Java: String.join(",", items)
来源：http://caa.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://rml.wangdashe.top

Ruby: items.join(",")
来源：http://wbt.zdqjudy.top

C#:   string.Join(",", items)
来源：http://dgx.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://jbb.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uiq.hywenlv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uww.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://hah.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://ddr.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://ngm.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://ooo.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://owv.shuidangran.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rot.fktsv.cn

[E10] 左侧补零 / 定长填充
来源：http://fzl.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nkm.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vpa.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://gnd.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://eml.hnqzz.top

Java: String.format("%03d", 7)
来源：http://xmn.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://iak.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://epb.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hoo.jianghu66.top

[E11] 反转字符串
来源：http://ggo.cqqwz.cn

Py:   s[::-1]
来源：http://nqw.hnqzz.top

PHP:  strrev($s);
来源：http://fhu.yuxming.cn

JS:   [...s].reverse().join("")
来源：http://akl.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://jtg.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vjm.hysaishi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gqi.cashguo.top

Ruby: s.reverse
来源：http://sqn.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://hkd.fktsv.cn

[E12] 统计某字符出现次数
来源：http://fqc.guannengcc.top

Py:   s.count("a")
来源：http://dim.sweek.top

PHP:  substr_count($s, "a");
来源：http://kto.nwbrower.top

JS:   s.split("a").length - 1
来源：http://qmz.andypj.xyz

TS:   s.split("a").length - 1
来源：http://prg.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://elr.jianghu66.top

Go:   strings.Count(s, "a")
来源：http://tpa.52xcode.cn

Ruby: s.count("a")
来源：http://hly.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://con.bbcook.cn

[E13] 逐字符遍历
来源：http://jnk.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://yrf.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://erw.sxryk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cef.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://aum.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nto.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://spx.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://krx.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rkc.epnwcf.com

[E14] URL 编码与 Base64
来源：http://gou.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jqu.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://api.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mig.vqdsnc.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jtp.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zkr.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mcz.fzhhl.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cpf.cheryme.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fvh.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://uwx.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rrd.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://alp.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ckq.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://idi.tianlin.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ckz.fehbvm.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uza.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://evu.jlsjyb.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sdy.sysykeji.top

[E16] 数字千分位
来源：http://lds.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://ryp.guowangkeji.top

PHP:  number_format(1234567);
来源：http://nou.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dpu.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gfd.nwbrower.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jmp.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fte.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://van.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://jqx.nwbrower.top

[E17] 首字母大写
来源：http://mmo.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qxv.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ffe.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rec.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vue.yfazqb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bvj.sweek.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yzs.ivvv.top

Ruby: s.capitalize
来源：http://fjk.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ybz.sjlbkw.cn

[E18] 模板占位符替换
来源：http://rvx.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mvs.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zmx.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://peq.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tea.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mzx.yj20258888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vdu.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ccb.shangyingyoupin.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pal.yonumen.top

[E19] 多行文本按行拆分
来源：http://mxc.0kj1m.cn

Py:   s.splitlines()
来源：http://mxx.hcnkem.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gkh.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://nwq.chenlongwang.top

TS:   s.split(/\r?\n/)
来源：http://atv.aibaodan.cn

Java: s.lines().toList()
来源：http://yqv.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://otb.yj20258.top

Ruby: s.lines
来源：http://blq.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://jat.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://fgy.fengsongda.top

Py:   if not s:
来源：http://gzp.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yms.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hks.cqqwz.cn

TS:   if (s === "") {}
来源：http://dgk.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://sky.guannengcc.top

Go:   if s == "" {}
来源：http://smn.guannengcc.top

Ruby: if s.empty?
来源：http://sej.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zlh.daxiang520.top

[E21] 超长截断加省略号
来源：http://ytl.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ntp.hfpthk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ood.hywenlv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gfc.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ihr.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kpa.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://qny.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xcy.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qop.fktsv.cn

[E22] 字节长度与字符长度
来源：http://orr.cheryme.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gin.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pge.yanxiufei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://igj.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oci.yj20258.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ocl.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://feu.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://nsy.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ntz.tianlin.xyz

================================================================================
来源：http://ywq.dianchejie.cn

F. 文件与目录
来源：http://jsp.chenlongwang.top

================================================================================
来源：http://mca.hysaishi.cn

[F01] 读取整个文件
来源：http://ylp.cashguo.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cyd.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://awx.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xsa.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zln.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://evb.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ddt.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://vlw.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://eqr.ctjpmb.com

[F02] 逐行读取文件
来源：http://egq.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yys.0kj1m.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cnh.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://djz.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xeh.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qos.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ojp.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wmb.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cfo.ivvv.top

[F03] 写入文件（覆盖）
来源：http://kph.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ivb.smart0.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://tvz.yj202588.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ofp.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cnb.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://deu.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xhc.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://cvr.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sfd.nanxinkj.top

[F04] 追加写入文件
来源：http://vvy.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pwr.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rmk.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xlf.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://czm.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zml.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vad.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gce.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://miu.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://mfi.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dea.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://lqd.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://qqk.yuanzhike.top

TS:   fs.existsSync("a.txt")
来源：http://yur.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://jrd.fanxiaobao.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bmm.sweek.top

Ruby: File.exist?("a.txt")
来源：http://mqb.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://ndn.yfazqb.com

[F06] 删除文件
来源：http://yey.jiagoushi.top

Py:   os.remove("a.txt")
来源：http://xrh.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://pgp.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sij.ybcxt.top

TS:   fs.unlinkSync("a.txt")
来源：http://ixw.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qgn.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://lvv.andypj.xyz

Ruby: File.delete("a.txt")
来源：http://vhz.c1oappe.top

C#:   File.Delete("a.txt");
来源：http://fgb.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://uuv.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://evq.chenjidiqi.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xuy.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gpf.meibo888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fez.zhixingplan.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fpn.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ajl.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bnq.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wwt.fktsv.cn

[F08] 遍历目录
来源：http://bvq.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://wwe.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xdt.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://phc.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://qjm.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xhe.zhengqikj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ywx.cashguo.top

Ruby: Dir.children("dir")
来源：http://qfy.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://xlj.dashuyun.cn

[F09] 获取文件大小
来源：http://mwi.fehbvm.com

Py:   os.path.getsize("a.txt")
来源：http://xnw.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://eef.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://pim.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://apk.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kwf.chenzaomai.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zqz.nwbrower.top

Ruby: File.size("a.txt")
来源：http://gjg.bbcook.cn


<!-- 参考信息 -->