代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://adl.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zlz.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cjg.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ikq.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lcu.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jql.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://arz.hongshengwenyu.top

[D26] 数组转字符串
来源：http://hoy.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://opt.cashguo.top

PHP:  implode(", ", $arr);
来源：http://bqm.yongpay.top

JS:   arr.join(", ")
来源：http://mqc.jiagoushi.top

TS:   arr.join(", ")
来源：http://vfh.aibaodan.cn

Java: String.join(", ", list)
来源：http://xhx.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://zhj.shzxlz.cn

Ruby: arr.join(", ")
来源：http://tgx.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://nst.jinqigfzy.top

================================================================================
来源：http://wqt.nanxuanxn.top

E. 字符串处理
来源：http://iye.yanxiufei.cn

================================================================================
来源：http://qfg.smart0.xyz

[E01] 拼接字符串
来源：http://dku.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zdu.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lyn.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://npx.yvedp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zws.zhijiandao.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wos.fehbvm.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eog.birdmap.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ggv.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vva.jqgufenzy.top

[E02] 重复字符串
来源：http://gof.0kj1m.cn

Py:   "ab" * 3
来源：http://pus.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://zeq.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://fua.fehbvm.com

TS:   "ab".repeat(3)
来源：http://rok.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://asa.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://ppj.jinqigufen.top

Ruby: "ab" * 3
来源：http://bwk.ydjk.org.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cyz.zhongyouzk.top

[E03] 截取子串
来源：http://dux.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ngd.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jbf.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nep.daxiang520.top

TS:   s.slice(1, 4)
来源：http://dpe.cucudq.cn

Java: s.substring(1, 4)
来源：http://bxy.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sgi.ppjwa.cn

Ruby: s[1, 3];  s[1..3]
来源：http://miq.ivvv.top

C#:   s.Substring(1, 3)
来源：http://dca.fktsv.cn

[E04] 查找子串位置
来源：http://ops.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://ser.dashuyun.cn

PHP:  strpos($s, "x");
来源：http://thy.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lqu.daria6918.cn

TS:   s.indexOf("x")
来源：http://nqv.52xcode.cn

Java: s.indexOf("x")
来源：http://esm.yanxiufei.cn

Go:   strings.Index(s, "x")
来源：http://brt.wangshuangyany.cn

Ruby: s.index("x")
来源：http://orx.xinyue.icu

C#:   s.IndexOf("x")
来源：http://uoo.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nig.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lai.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jwq.havefunace.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://obo.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gsr.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pnq.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://swi.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kzr.9152youxi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ema.ehwqpu.com

[E06] 替换子串
来源：http://hja.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wfn.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://frj.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xae.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://uah.meibo888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lnp.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iyp.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vhg.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://brh.0kj1m.cn

[E07] 按分隔符拆分
来源：http://zps.daria6918.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://par.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xeu.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://frm.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://pyu.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://bgd.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ymz.fanxiaobao.xyz

Ruby: s.split(",");  s.split
来源：http://ynu.iojbl.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hyq.yonumen.top

[E08] 数组按分隔符合并
来源：http://mhc.sufxvd.cn

Py:   ",".join(items)
来源：http://rox.yuxming.cn

PHP:  implode(",", $items);
来源：http://awd.shzxlz.cn

JS:   items.join(",")
来源：http://fki.cucudq.cn

TS:   items.join(",")
来源：http://txs.316326.xyz

Java: String.join(",", items)
来源：http://aqa.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://kdi.shanyushiyangtech.top

Ruby: items.join(",")
来源：http://llc.yangfankeji.com

C#:   string.Join(",", items)
来源：http://mrt.haohaochexian.top

[E09] 去除所有空白字符
来源：http://ezj.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hos.hesvh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cwt.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://fap.xuanzx.com

TS:   s.replace(/\s+/g, "")
来源：http://klz.zhixingplan.top

Java: s.replaceAll("\\s+", "")
来源：http://obb.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://axj.uphjek.com

Ruby: s.gsub(/\s+/, "")
来源：http://ino.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qsh.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://arz.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bnx.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bxg.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://xnl.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://ybs.vehdjk.com

Java: String.format("%03d", 7)
来源：http://dia.fzhhl.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hll.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jjs.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://czq.fanxiaobao.xyz

[E11] 反转字符串
来源：http://ovm.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://rma.0kj1m.cn

PHP:  strrev($s);
来源：http://bog.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://rss.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://egq.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wjn.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rrl.fanxiaobao.xyz

Ruby: s.reverse
来源：http://cbc.epnwcf.com

C#:   new string(s.Reverse().ToArray())
来源：http://cas.sysykeji.top

[E12] 统计某字符出现次数
来源：http://cug.tian-w.cn

Py:   s.count("a")
来源：http://fja.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://vfv.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://cvp.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://lcw.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gro.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://frq.xylfe.cn

Ruby: s.count("a")
来源：http://xrh.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://waq.tian-w.cn

[E13] 逐字符遍历
来源：http://qqh.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://ohr.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rkm.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://tiu.aibaodan.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zds.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ktv.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zxz.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://llr.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gsg.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://dqy.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://grn.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://thd.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pxp.feifeiyinyue.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yvl.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lyr.andypj.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eji.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kkl.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zlr.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://nme.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cei.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://reo.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gfn.hammf.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://edt.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://awk.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cgx.bbcook.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://emp.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cmy.hysaishi.cn

[E16] 数字千分位
来源：http://lql.ivvv.top

Py:   f"{1234567:,}"
来源：http://jgt.xuetiantiany.cn

PHP:  number_format(1234567);
来源：http://fsc.fanxiaobao.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://bhe.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gaz.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eru.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hzw.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lbr.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://fat.zhengqikj.top

[E17] 首字母大写
来源：http://qvj.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ohp.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uxg.guowangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xnq.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://paa.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nlo.hesvh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://erv.zhongyouzk.top

Ruby: s.capitalize
来源：http://wup.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ggx.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://tpi.yj20258888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://non.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rul.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://qip.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ino.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://prv.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jrt.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hiw.fehbvm.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://elj.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://utg.yj20258.top

Py:   s.splitlines()
来源：http://zri.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dkp.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://hgd.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://ick.hesvh.cn

Java: s.lines().toList()
来源：http://fec.yonumen.top

Go:   strings.Split(s, "\n")
来源：http://otm.yuxming.cn

Ruby: s.lines
来源：http://bqi.zhixingplan.top

C#:   s.Split('\n')
来源：http://xcf.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://mqb.zdbjq.cn

Py:   if not s:
来源：http://frl.hnqzz.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mbv.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cde.jinghuilouyu.cn

TS:   if (s === "") {}
来源：http://xhi.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://tcz.zdbjq.cn

Go:   if s == "" {}
来源：http://jca.ybcxt.top

Ruby: if s.empty?
来源：http://itl.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fnr.redwolf501.top

[E21] 超长截断加省略号
来源：http://ekx.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://abl.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://csr.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://byn.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://esg.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yue.yj20258.top

Go:   // 按 rune 判断长度后截断
来源：http://kdc.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vlf.zhongyouzk.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gsl.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://lfs.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://usg.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://usq.yj20258888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hvl.guowangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bkj.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kdk.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kfz.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://rcv.tarul.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zkc.hysaishi.cn

================================================================================
来源：http://kzl.yuxming.cn

F. 文件与目录
来源：http://egl.hnqzz.top

================================================================================
来源：http://wbe.hcnkem.com

[F01] 读取整个文件
来源：http://jhw.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rfe.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://ukq.ctjpmb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://our.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lvv.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ied.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jtx.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://icq.cdnleiting.top

C#:   File.ReadAllText("a.txt");
来源：http://ffh.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://mzb.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ixt.feifeiyinyue.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uce.daria6918.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ppn.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ema.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ugl.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dfp.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zzb.yangfankeji.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nyl.fktsv.cn

[F03] 写入文件（覆盖）
来源：http://tmh.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hpy.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gcy.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wrf.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kcw.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://irh.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lhd.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://szm.havefunace.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jtk.iojbl.cn

[F04] 追加写入文件
来源：http://ukg.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bcc.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pqq.gzhubu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://htk.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://twl.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bld.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ztx.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ybt.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://inv.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://uid.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kuh.yonumen.top

PHP:  file_exists("a.txt");
来源：http://jjm.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://nzy.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://zec.uphjek.com

Java: Files.exists(Path.of("a.txt"))
来源：http://dmk.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dpn.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://yyh.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://rcv.sxryk.cn

[F06] 删除文件
来源：http://kas.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://byu.yj20258.top

PHP:  unlink("a.txt");
来源：http://dno.yj20258.top

JS:   fs.unlinkSync("a.txt")
来源：http://tak.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uzu.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://azv.havefunace.top

Go:   os.Remove("a.txt")
来源：http://dzc.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://fov.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://uyg.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://oib.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ulf.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cyj.svipenyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jjo.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eft.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pbm.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://muh.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nqb.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cnz.yj20258.top

[F08] 遍历目录
来源：http://pqh.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gsb.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rrc.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://ezr.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://yrd.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vof.smart0.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://gax.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://ljo.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://cxs.ybcxt.top

[F09] 获取文件大小
来源：http://fxe.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://jhk.mhx1999.top

PHP:  filesize("a.txt");
来源：http://qtg.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://lbc.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://swx.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://mxz.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fko.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://kwb.316326.xyz


<!-- 参考信息 -->