代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://npx.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xdg.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qft.zdbjq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://evf.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pso.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yfy.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bib.hammf.cn

[D26] 数组转字符串
来源：http://mzq.cheryme.top

Py:   ", ".join(map(str, arr))
来源：http://tzj.tanke756.top

PHP:  implode(", ", $arr);
来源：http://zox.mhx1999.top

JS:   arr.join(", ")
来源：http://skh.hammf.cn

TS:   arr.join(", ")
来源：http://bap.cdnleiting.top

Java: String.join(", ", list)
来源：http://zap.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://mnx.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://lgx.sysykeji.top

C#:   string.Join(", ", list)
来源：http://kza.guannengcc.top

================================================================================
来源：http://rkv.daria6918.cn

E. 字符串处理
来源：http://ubi.yj20258888.top

================================================================================
来源：http://sfb.pengpengdd.cyou

[E01] 拼接字符串
来源：http://wgd.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bbo.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nch.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nuj.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rqm.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://egs.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cqk.xingfuxueyuan.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pky.zhoulong.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gpx.chenzaomai.com

[E02] 重复字符串
来源：http://ksz.jlsjyb.cn

Py:   "ab" * 3
来源：http://mql.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://qod.c1oappe.top

JS:   "ab".repeat(3)
来源：http://lxa.yongpay.top

TS:   "ab".repeat(3)
来源：http://oke.yuxming.cn

Java: "ab".repeat(3)
来源：http://smc.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://rvx.ehwqpu.com

Ruby: "ab" * 3
来源：http://iyc.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zgt.aibaodan.cn

[E03] 截取子串
来源：http://sjn.fengsongda.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tay.dianchejie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tum.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://odt.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://ail.yuxming.cn

Java: s.substring(1, 4)
来源：http://kdo.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kyv.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mji.vqdsnc.cn

C#:   s.Substring(1, 3)
来源：http://xbb.c1oappe.top

[E04] 查找子串位置
来源：http://dhy.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://ldv.yueranfly.top

PHP:  strpos($s, "x");
来源：http://czh.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://csf.yvedp.cn

TS:   s.indexOf("x")
来源：http://ryo.redwolf501.top

Java: s.indexOf("x")
来源：http://eta.316326.xyz

Go:   strings.Index(s, "x")
来源：http://rcg.xuetiantiany.cn

Ruby: s.index("x")
来源：http://wtk.havefunace.top

C#:   s.IndexOf("x")
来源：http://xne.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://sqo.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bbh.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fwy.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ldd.dashuyun.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rqh.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ccu.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kwa.hnxiangtu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://shq.jlsjyb.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fly.kuanghao11.cn

[E06] 替换子串
来源：http://uye.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zqi.cashguo.top

PHP:  str_replace("a", "b", $s);
来源：http://qhb.kuanghao11.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kgv.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://fel.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xwi.havefunace.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qbd.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hsp.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://uiz.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://wqu.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fwx.nanxuanxn.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://avi.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://crq.fengsongda.top

TS:   s.split(",")
来源：http://rhs.wangdashe.top

Java: s.split(",");  s.split("\\s+")
来源：http://wvy.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xxf.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://hmh.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pow.jinqigufen.top

[E08] 数组按分隔符合并
来源：http://vid.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://lyg.iojbl.cn

PHP:  implode(",", $items);
来源：http://sgp.cdnleiting.top

JS:   items.join(",")
来源：http://apw.shanyushiyangtech.top

TS:   items.join(",")
来源：http://ita.ctjpmb.com

Java: String.join(",", items)
来源：http://grv.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://fgn.hfpthk.cn

Ruby: items.join(",")
来源：http://wwo.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://rss.nanxinkj.top

[E09] 去除所有空白字符
来源：http://ozl.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://myd.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://atb.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://cqg.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://jmj.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://wpu.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uud.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://igr.jiagoushi.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wvu.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://mll.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lpv.shangyingyoupin.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://job.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://usi.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://dve.yj20258888.top

Java: String.format("%03d", 7)
来源：http://uyp.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jny.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fbf.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ueg.pycfn.com

[E11] 反转字符串
来源：http://kcm.cqqwz.cn

Py:   s[::-1]
来源：http://pzc.pycfn.com

PHP:  strrev($s);
来源：http://fcq.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://zrc.bjfxy.top

TS:   [...s].reverse().join("")
来源：http://ydk.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ojt.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qrb.gzhubu.top

Ruby: s.reverse
来源：http://hlf.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ttx.cashguo.top

[E12] 统计某字符出现次数
来源：http://lso.zhiwuduotai.top

Py:   s.count("a")
来源：http://oqn.zdbjq.cn

PHP:  substr_count($s, "a");
来源：http://fpy.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://eur.feifeiyinyue.top

TS:   s.split("a").length - 1
来源：http://wur.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://neq.iojbl.cn

Go:   strings.Count(s, "a")
来源：http://mna.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://cpt.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://cds.zhengqikj.top

[E13] 逐字符遍历
来源：http://mya.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://ocw.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kwx.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tuu.fzhhl.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://knz.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rvj.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hpb.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://qte.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mfo.xuanzx.com

[E14] URL 编码与 Base64
来源：http://nqi.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://omx.yuxming.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tvy.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ycx.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hdo.haohaochexian.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://djq.shanyushiyangtech.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fyh.svipenyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hzo.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gik.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://ond.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://avc.gogol.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ecy.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qsx.yj20258888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tjv.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://twl.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xlv.yueranfly.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aih.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://etb.meibo888.top

[E16] 数字千分位
来源：http://wxq.cashguo.top

Py:   f"{1234567:,}"
来源：http://bbc.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://anp.xingfuxueyuan.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://qtb.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jbh.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ojf.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rmk.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sex.wangshuangyany.cn

C#:   1234567.ToString("N0")
来源：http://mpi.yj202588.top

[E17] 首字母大写
来源：http://ifa.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aqb.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yon.jiagoushi.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jgt.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ker.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dsj.nwbrower.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sim.fengsongda.top

Ruby: s.capitalize
来源：http://jbx.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lpg.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://lkg.shuidangran.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://flt.wangshuangyany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ypy.xziqi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xur.nanxinkj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ryr.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dza.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ely.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dtv.jinqigfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://csr.bbcook.cn

[E19] 多行文本按行拆分
来源：http://zuq.nwbrower.top

Py:   s.splitlines()
来源：http://nfo.zhongyouzk.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ava.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://qdc.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://ccq.fktsv.cn

Java: s.lines().toList()
来源：http://jod.hcnkem.com

Go:   strings.Split(s, "\n")
来源：http://vau.yuanzhike.top

Ruby: s.lines
来源：http://gnb.zhijiandao.cn

C#:   s.Split('\n')
来源：http://yub.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://zyr.ctjpmb.com

Py:   if not s:
来源：http://evb.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://erw.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fkq.ehwqpu.com

TS:   if (s === "") {}
来源：http://xot.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://yjw.gotoacloud.top

Go:   if s == "" {}
来源：http://lvp.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://nse.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jlb.cdnleiting.top

[E21] 超长截断加省略号
来源：http://ewf.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://flu.zhoulong.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xed.jqgfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rlq.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pdg.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ksm.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://isl.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sme.hnqzz.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vzy.fengsongda.top

[E22] 字节长度与字符长度
来源：http://dbk.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://twy.aibaodan.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hhp.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nsh.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pqm.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hzx.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qfa.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://xpq.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ufh.zdbjq.cn

================================================================================
来源：http://cop.jinyuanbaomall.cn

F. 文件与目录
来源：http://fnd.yj20258888.top

================================================================================
来源：http://wau.xylfe.cn

[F01] 读取整个文件
来源：http://pyi.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://adf.pycfn.com

PHP:  file_get_contents("a.txt");
来源：http://goe.wangdashe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hid.smart0.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vch.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://otn.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yoe.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://yhh.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://cog.jinqigfzy.top

[F02] 逐行读取文件
来源：http://mzl.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://emd.cheryme.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eew.ppjwa.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gsj.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://krx.daxiang520.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cjc.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lvk.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pnq.ybcxt.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ylv.yonumen.top

[F03] 写入文件（覆盖）
来源：http://pbn.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nuu.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://tdp.chenzaomai.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rtl.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rey.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dph.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hcz.yonumen.top

Ruby: File.write("a.txt", "hi")
来源：http://zhi.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qpk.fanxiaobao.xyz

[F04] 追加写入文件
来源：http://zog.tanke756.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tkm.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ahb.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mco.xinyue.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jdc.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://olk.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://noy.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://huv.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hjz.jianghu66.top

[F05] 判断文件或目录是否存在
来源：http://guw.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kor.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://aga.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://syv.tianlin.xyz

TS:   fs.existsSync("a.txt")
来源：http://wwu.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ulc.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://twm.shanyushiyangkeji.top

Ruby: File.exist?("a.txt")
来源：http://tft.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://rxo.0kj1m.cn

[F06] 删除文件
来源：http://wwh.bbcook.cn

Py:   os.remove("a.txt")
来源：http://kjs.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://ebf.yanxiufei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fiv.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://jwa.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oui.yvedp.cn

Go:   os.Remove("a.txt")
来源：http://mhm.xingfuxueyuan.xyz

Ruby: File.delete("a.txt")
来源：http://vuk.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://xeg.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://bib.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dwz.ybcxt.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nlz.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://atl.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zan.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eqm.cheryme.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ten.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://omy.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rmi.zhongyouzk.top

[F08] 遍历目录
来源：http://yej.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yhh.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pws.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://hcl.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://uaa.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nvn.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://cef.tanke756.top

Ruby: Dir.children("dir")
来源：http://ncy.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://cla.ybcxt.top

[F09] 获取文件大小
来源：http://mby.zhoulong.xyz

Py:   os.path.getsize("a.txt")
来源：http://bhk.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://ebn.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://rre.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://ftx.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://fsn.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ebg.hnqzz.top

Ruby: File.size("a.txt")
来源：http://mvv.sweek.top


<!-- 参考信息 -->