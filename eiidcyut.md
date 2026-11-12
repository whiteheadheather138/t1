代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gzt.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lpw.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://end.zhoulong.xyz

[D26] 数组转字符串
来源：http://pui.jinqigufen.top

Py:   ", ".join(map(str, arr))
来源：http://jsg.fktsv.cn

PHP:  implode(", ", $arr);
来源：http://acp.zdqjudy.top

JS:   arr.join(", ")
来源：http://qxx.fehbvm.com

TS:   arr.join(", ")
来源：http://tac.bjfxy.top

Java: String.join(", ", list)
来源：http://ovr.zhiwuduotai.top

Go:   strings.Join(strs, ", ")
来源：http://ujv.uphjek.com

Ruby: arr.join(", ")
来源：http://eop.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://sdk.52xcode.cn

================================================================================
来源：http://qsu.zhixingplan.top

E. 字符串处理
来源：http://yez.haohaochexian.top

================================================================================
来源：http://quz.jianghu66.top

[E01] 拼接字符串
来源：http://mzd.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ktw.jlsjyb.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fye.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pkg.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xrs.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vch.fehbvm.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yja.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vxf.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uth.iojbl.cn

[E02] 重复字符串
来源：http://fzw.cucudq.cn

Py:   "ab" * 3
来源：http://ujt.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://vhi.bjfxy.top

JS:   "ab".repeat(3)
来源：http://hyy.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://nsj.hysaishi.cn

Java: "ab".repeat(3)
来源：http://iuo.kuanghao11.cn

Go:   strings.Repeat("ab", 3)
来源：http://dlp.gotoacloud.top

Ruby: "ab" * 3
来源：http://svw.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cdi.hongshengwenyu.top

[E03] 截取子串
来源：http://obo.jqgfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wiy.tianlin.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wqh.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zwi.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://fbt.xuanzx.com

Java: s.substring(1, 4)
来源：http://wlr.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ipe.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://eva.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://kud.yangfankeji.com

[E04] 查找子串位置
来源：http://ciy.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://mlw.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://hli.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qri.hnqzz.top

TS:   s.indexOf("x")
来源：http://lax.smart0.xyz

Java: s.indexOf("x")
来源：http://puw.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://yqf.yj20258888.top

Ruby: s.index("x")
来源：http://wkh.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://bkm.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://zho.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ufp.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rwh.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uaf.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://xfe.tianlin.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jfe.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aeq.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fsl.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gqe.zhixingplan.top

[E06] 替换子串
来源：http://rja.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oag.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://aab.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fug.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://tsc.jinghuilouyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xwr.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kuj.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://opc.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://qac.nanxinkj.top

[E07] 按分隔符拆分
来源：http://amb.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://atb.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ijl.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://jde.52xcode.cn

TS:   s.split(",")
来源：http://lou.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://vhy.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zpy.hnxiangtu.top

Ruby: s.split(",");  s.split
来源：http://kyp.zhongyouzk.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iyz.fanxiaobao.xyz

[E08] 数组按分隔符合并
来源：http://ztw.ydzc1.top

Py:   ",".join(items)
来源：http://xzd.iojbl.cn

PHP:  implode(",", $items);
来源：http://bku.52xcode.cn

JS:   items.join(",")
来源：http://ghr.hcnkem.com

TS:   items.join(",")
来源：http://qbb.svipenyu.cn

Java: String.join(",", items)
来源：http://xkp.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://bnd.quarkkingdee.top

Ruby: items.join(",")
来源：http://nai.andypj.xyz

C#:   string.Join(",", items)
来源：http://bun.zhaomingkeji.xyz

[E09] 去除所有空白字符
来源：http://doc.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jgg.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mni.wangdashe.top

JS:   s.replace(/\s+/g, "")
来源：http://rnc.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://coi.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://jiy.cdnleiting.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://iah.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://ftu.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://usk.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://zcw.quarkkingdee.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hkz.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fki.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://hkq.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://ime.guannengcc.top

Java: String.format("%03d", 7)
来源：http://eam.jinqigufen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://dpu.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://adz.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kbd.aizwys.cn

[E11] 反转字符串
来源：http://ida.wangshuangyany.cn

Py:   s[::-1]
来源：http://egy.c1oappe.top

PHP:  strrev($s);
来源：http://gdp.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://vuf.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://dvg.iojbl.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qcn.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nyx.uphjek.com

Ruby: s.reverse
来源：http://rsc.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://htz.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://zgg.gaohongyu789.top

Py:   s.count("a")
来源：http://sfk.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://wxc.yuanzhike.top

JS:   s.split("a").length - 1
来源：http://xsk.xziqi.cn

TS:   s.split("a").length - 1
来源：http://sdt.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://psl.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://pjg.guowangkeji.top

Ruby: s.count("a")
来源：http://eeq.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://jkz.zhengqikj.top

[E13] 逐字符遍历
来源：http://tdi.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://sgc.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ezi.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tlw.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dze.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tij.jinqigufen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://idi.haohaochexian.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oso.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rxh.yangfankeji.com

[E14] URL 编码与 Base64
来源：http://kqi.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dyw.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rqf.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tnf.zdbjq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tuz.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kdl.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nag.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jjx.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gtx.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://lcy.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ffx.hesvh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rek.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lot.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nfj.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ghd.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vsc.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cpc.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fxp.yfazqb.com

[E16] 数字千分位
来源：http://lob.ybcxt.top

Py:   f"{1234567:,}"
来源：http://hvq.ehwqpu.com

PHP:  number_format(1234567);
来源：http://zsv.fzhhl.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ncp.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fjh.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gef.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vro.svipenyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kve.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://zgy.dashuyun.cn

[E17] 首字母大写
来源：http://okv.vehdjk.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://idc.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dxx.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lqw.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jie.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kmq.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dvw.hysaishi.cn

Ruby: s.capitalize
来源：http://rbd.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bzd.hfpthk.cn

[E18] 模板占位符替换
来源：http://jnj.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oen.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hdo.yangfankeji.com

JS:   tpl.replaceAll("{name}", name)
来源：http://txo.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://min.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nbp.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xnd.daxiang520.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ydz.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rvj.ybcxt.top

[E19] 多行文本按行拆分
来源：http://lly.fktsv.cn

Py:   s.splitlines()
来源：http://dva.wangshuangyany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kzt.zhoulong.xyz

JS:   s.split(/\r?\n/)
来源：http://kwr.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://lqi.mhx1999.top

Java: s.lines().toList()
来源：http://pcd.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://gvs.ydjk.org.cn

Ruby: s.lines
来源：http://ruj.gotoacloud.top

C#:   s.Split('\n')
来源：http://hfi.cqqwz.cn

[E20] 判断字符串是否为空
来源：http://zbk.yj20258888.top

Py:   if not s:
来源：http://rfh.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://moq.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yml.fzhhl.top

TS:   if (s === "") {}
来源：http://rsq.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://mad.jiagoushi.top

Go:   if s == "" {}
来源：http://rop.aibaodan.cn

Ruby: if s.empty?
来源：http://lbd.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bjb.zdqjudy.top

[E21] 超长截断加省略号
来源：http://jfh.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rsc.bbcook.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wbe.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qbo.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yzw.hfpthk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qfg.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://afl.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://trg.ydjk.org.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tpl.0kj1m.cn

[E22] 字节长度与字符长度
来源：http://rne.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ymv.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uhx.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://poa.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ekq.yongpay.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://atu.52xcode.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ccu.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://wpx.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ffi.jinghuilouyu.cn

================================================================================
来源：http://mre.zhijiandao.cn

F. 文件与目录
来源：http://ftz.jinqigfzy.top

================================================================================
来源：http://vma.gotoacloud.top

[F01] 读取整个文件
来源：http://wbm.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gyq.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://agk.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tew.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cas.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://jbc.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kdr.yvedp.cn

Ruby: File.read("a.txt")
来源：http://cep.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://usv.tian-w.cn

[F02] 逐行读取文件
来源：http://fmc.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yjj.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tef.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://guu.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ofo.xuetiantiany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ypu.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jnf.ybcxt.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vim.hnqzz.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pyz.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://niv.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ivp.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jff.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ten.cheryme.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iau.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vvr.jianghu66.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jsi.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://lnd.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hap.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://unm.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vvj.nanxuanxn.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gmu.ydzc1.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cja.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zss.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gje.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nel.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://txe.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sos.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://nrk.hammf.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dfc.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://ofs.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://nww.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://vls.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sdr.mhx1999.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ydf.cucudq.cn

Ruby: File.exist?("a.txt")
来源：http://fys.nanxinkj.top

C#:   File.Exists("a.txt")
来源：http://kqs.316326.xyz

[F06] 删除文件
来源：http://cgv.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://klr.hysaishi.cn

PHP:  unlink("a.txt");
来源：http://fdr.ppjwa.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wfc.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://sib.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vhn.zdbjq.cn

Go:   os.Remove("a.txt")
来源：http://rue.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://tin.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://hkv.smart0.xyz

[F07] 创建目录（含多级）
来源：http://pzc.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xca.yvedp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lsp.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://utm.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tfc.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ntr.tianlin.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zmi.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bvg.yonumen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nib.cashguo.top

[F08] 遍历目录
来源：http://nsj.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ggm.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://plr.redwolf501.top

JS:   fs.readdirSync("dir")
来源：http://zfx.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://psu.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cfg.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zmd.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://jyl.feifeiyinyue.top

C#:   Directory.GetFiles("dir")
来源：http://ybw.yuxming.cn

[F09] 获取文件大小
来源：http://uzl.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://xbw.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://pyx.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://jnb.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://mmq.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://oqa.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mwp.hnqzz.top

Ruby: File.size("a.txt")
来源：http://mml.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://tob.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://azs.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gdm.jinqigfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tqk.kuanghao11.cn


<!-- 参考信息 -->