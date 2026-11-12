代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tyh.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wlb.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qjt.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aju.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zvf.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wlb.jinghuilouyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rks.andypj.xyz

[D26] 数组转字符串
来源：http://dvq.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://las.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://qhy.zycfv.cn

JS:   arr.join(", ")
来源：http://jvj.hywenlv.cn

TS:   arr.join(", ")
来源：http://iye.tarul.cn

Java: String.join(", ", list)
来源：http://fbl.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://yji.sweek.top

Ruby: arr.join(", ")
来源：http://wft.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://uhv.hfpthk.cn

================================================================================
来源：http://pqj.gzhubu.top

E. 字符串处理
来源：http://owm.bjfxy.top

================================================================================
来源：http://wlv.0kj1m.cn

[E01] 拼接字符串
来源：http://iyw.jiagoushi.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pio.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://clb.0kj1m.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://juu.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ckm.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ffe.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://idy.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fpe.fehbvm.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dbr.gogol.net.cn

[E02] 重复字符串
来源：http://jpg.yj20258.top

Py:   "ab" * 3
来源：http://lpf.svipenyu.cn

PHP:  str_repeat("ab", 3);
来源：http://qqy.zhengqikj.top

JS:   "ab".repeat(3)
来源：http://gmg.xuanzx.com

TS:   "ab".repeat(3)
来源：http://uvs.fktsv.cn

Java: "ab".repeat(3)
来源：http://uta.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://dsz.cdnleiting.top

Ruby: "ab" * 3
来源：http://pdr.jinyuanbaomall.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tdq.dianchejie.cn

[E03] 截取子串
来源：http://rjb.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xqp.uphjek.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mat.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zid.zhaomingkeji.xyz

TS:   s.slice(1, 4)
来源：http://lpn.xziqi.cn

Java: s.substring(1, 4)
来源：http://scx.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ypj.yonumen.top

Ruby: s[1, 3];  s[1..3]
来源：http://iiv.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://qef.tarul.cn

[E04] 查找子串位置
来源：http://xrn.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://sth.fehbvm.com

PHP:  strpos($s, "x");
来源：http://qdo.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xsz.yj202588.top

TS:   s.indexOf("x")
来源：http://srv.daxiang520.top

Java: s.indexOf("x")
来源：http://flp.yongpay.top

Go:   strings.Index(s, "x")
来源：http://evu.gzhubu.top

Ruby: s.index("x")
来源：http://qeq.wangshuangyany.cn

C#:   s.IndexOf("x")
来源：http://esg.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oxd.kuanghao11.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vvx.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xrm.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://flv.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://euy.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nsx.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ucr.nanxuanxn.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rax.shzxlz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ybw.svipenyu.cn

[E06] 替换子串
来源：http://vye.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lvi.52xcode.cn

PHP:  str_replace("a", "b", $s);
来源：http://gzl.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gnh.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://stz.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://feo.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gyd.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mqu.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://qyv.birdmap.top

[E07] 按分隔符拆分
来源：http://nxh.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yaf.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rdt.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yxr.mhx1999.top

TS:   s.split(",")
来源：http://xyk.jinghuilouyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://evr.tian-w.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bkk.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://ovm.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rvv.andypj.xyz

[E08] 数组按分隔符合并
来源：http://bqy.jqgufenzy.top

Py:   ",".join(items)
来源：http://cue.zhijiandao.cn

PHP:  implode(",", $items);
来源：http://hky.9152youxi.cn

JS:   items.join(",")
来源：http://gzs.zhijiandao.cn

TS:   items.join(",")
来源：http://cuj.hesvh.cn

Java: String.join(",", items)
来源：http://izq.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://upo.aibaodan.cn

Ruby: items.join(",")
来源：http://iwd.smart0.xyz

C#:   string.Join(",", items)
来源：http://vmm.aizwys.cn

[E09] 去除所有空白字符
来源：http://xpr.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cry.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dog.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://mon.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://lmf.chenzaomai.com

Java: s.replaceAll("\\s+", "")
来源：http://gpx.redwolf501.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xkl.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://nuz.fktsv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xra.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://iuc.nwbrower.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jlq.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://idl.zycfv.cn

JS:   "7".padStart(3, "0")
来源：http://rwk.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://fbr.yueranfly.top

Java: String.format("%03d", 7)
来源：http://wso.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zer.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tia.sufxvd.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zlz.dianchejie.cn

[E11] 反转字符串
来源：http://csb.316326.xyz

Py:   s[::-1]
来源：http://onl.ivvv.top

PHP:  strrev($s);
来源：http://zhs.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://icr.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://kjr.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://pum.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nts.yvedp.cn

Ruby: s.reverse
来源：http://ema.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vmh.yvedp.cn

[E12] 统计某字符出现次数
来源：http://ojh.hnxiangtu.top

Py:   s.count("a")
来源：http://aad.hnxiangtu.top

PHP:  substr_count($s, "a");
来源：http://bca.c1oappe.top

JS:   s.split("a").length - 1
来源：http://ecs.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://iye.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oyk.cheryme.top

Go:   strings.Count(s, "a")
来源：http://eps.ivvv.top

Ruby: s.count("a")
来源：http://yuz.vqdsnc.cn

C#:   s.Count(c => c == 'a')
来源：http://ddo.xziqi.cn

[E13] 逐字符遍历
来源：http://hfa.andypj.xyz

Py:   for ch in s: print(ch)
来源：http://aql.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xbq.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://khy.xuetiantiany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://czi.zhixingplan.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gws.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wyc.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://kbv.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lut.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://vqi.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gcg.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nrj.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vnn.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rwx.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dos.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kdi.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tan.ctjpmb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://syp.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://dux.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tee.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eul.fktsv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mnp.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sct.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mkx.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gea.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cvl.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://exh.dashuyun.cn

[E16] 数字千分位
来源：http://iwb.yuanzhike.top

Py:   f"{1234567:,}"
来源：http://mbj.fehbvm.com

PHP:  number_format(1234567);
来源：http://xld.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vet.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bdz.fanxiaobao.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jfe.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fjr.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ydz.yongpay.top

C#:   1234567.ToString("N0")
来源：http://djn.svipenyu.cn

[E17] 首字母大写
来源：http://maa.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ikk.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hvo.cashguo.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mbq.xinyue.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hiy.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zow.gaohongyu789.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://npg.snrcjt.cn

Ruby: s.capitalize
来源：http://xra.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zbt.daria6918.cn

[E18] 模板占位符替换
来源：http://ajd.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bsx.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yio.bbcook.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://syt.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://ksy.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xbf.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lmm.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://edd.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wxz.daria6918.cn

[E19] 多行文本按行拆分
来源：http://tob.xuanzx.com

Py:   s.splitlines()
来源：http://lsw.yj20258.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eyi.redwolf501.top

JS:   s.split(/\r?\n/)
来源：http://jjp.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://zdt.fktsv.cn

Java: s.lines().toList()
来源：http://rhw.aibaodan.cn

Go:   strings.Split(s, "\n")
来源：http://qcr.hnqzz.top

Ruby: s.lines
来源：http://eed.vehdjk.com

C#:   s.Split('\n')
来源：http://sgw.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://ifh.yvedp.cn

Py:   if not s:
来源：http://olc.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://upn.jyoumei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oqk.zhijiandao.cn

TS:   if (s === "") {}
来源：http://vhc.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://ubp.fktsv.cn

Go:   if s == "" {}
来源：http://yhc.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://pzp.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mec.zhixingplan.top

[E21] 超长截断加省略号
来源：http://trk.xziqi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://grf.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ezt.zycfv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rnc.daria6918.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gcc.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tjy.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://mhe.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fmm.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cuw.mhx1999.top

[E22] 字节长度与字符长度
来源：http://qsk.cdnleiting.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sev.zhoulong.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sug.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xew.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hpd.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://csu.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sfs.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://qtu.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qvp.vqdsnc.cn

================================================================================
来源：http://ejc.mhx1999.top

F. 文件与目录
来源：http://nwu.xingfuxueyuan.xyz

================================================================================
来源：http://dey.chenlongwang.top

[F01] 读取整个文件
来源：http://awd.shuidangran.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oig.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://jpx.hnxiangtu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xwm.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jbz.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://chk.zhaomingkeji.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vgr.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://qgn.redwolf501.top

C#:   File.ReadAllText("a.txt");
来源：http://bop.andypj.xyz

[F02] 逐行读取文件
来源：http://dpo.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ala.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kdh.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yyt.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jpx.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ubb.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gbj.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://abd.xuetiantiany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cfc.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://yxi.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hun.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lih.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mqr.cucudq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bkx.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://daf.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xhr.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://qul.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://feo.chenzaomai.com

[F04] 追加写入文件
来源：http://mtc.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zha.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ttj.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://snf.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fcg.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://puh.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rfq.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jdj.hfpthk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fds.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://uot.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lsh.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://wmw.hysaishi.cn

JS:   fs.existsSync("a.txt")
来源：http://nwq.sufxvd.cn

TS:   fs.existsSync("a.txt")
来源：http://koj.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vwo.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pat.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://srm.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://cyp.ywan-chungtsiang.top

[F06] 删除文件
来源：http://biv.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://nqb.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://lgb.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://oek.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lly.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hkv.havefunace.top

Go:   os.Remove("a.txt")
来源：http://zac.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://htj.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://ymq.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://hsm.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://obo.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oyl.epnwcf.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dhz.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sef.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wix.hesvh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://loy.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://skt.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rcl.yj20258888.top

[F08] 遍历目录
来源：http://pmk.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zfi.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ccf.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://ttz.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://gys.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fhq.tianlin.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://oek.zycfv.cn

Ruby: Dir.children("dir")
来源：http://uuq.yfazqb.com

C#:   Directory.GetFiles("dir")
来源：http://rzk.tarul.cn

[F09] 获取文件大小
来源：http://dqk.sysykeji.top

Py:   os.path.getsize("a.txt")
来源：http://lnp.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://mtv.dianchejie.cn

JS:   fs.statSync("a.txt").size
来源：http://hri.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://syi.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://sbs.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://loy.ivvv.top

Ruby: File.size("a.txt")
来源：http://jkv.pycfn.com


<!-- 参考信息 -->