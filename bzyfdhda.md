代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://geg.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tjo.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zwv.shangyingyoupin.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ive.snrcjt.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yzc.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ygn.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://wse.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://otk.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nnm.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ujs.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jsb.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yte.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gbj.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rbn.chenlongwang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eiq.ybcxt.top

[D26] 数组转字符串
来源：http://zrs.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://xqv.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://uta.ydjk.org.cn

JS:   arr.join(", ")
来源：http://vrs.hcnkem.com

TS:   arr.join(", ")
来源：http://bpf.guowangkeji.top

Java: String.join(", ", list)
来源：http://nvf.hywenlv.cn

Go:   strings.Join(strs, ", ")
来源：http://zfz.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://wdv.hcnkem.com

C#:   string.Join(", ", list)
来源：http://cuc.smart0.xyz

================================================================================
来源：http://bll.cqqwz.cn

E. 字符串处理
来源：http://eun.aizwys.cn

================================================================================
来源：http://iid.0kj1m.cn

[E01] 拼接字符串
来源：http://rls.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tsb.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xxu.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dsx.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://npg.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ghw.uphjek.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kph.yuanzhike.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://imw.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jci.kuanghao11.cn

[E02] 重复字符串
来源：http://kul.meibo888.top

Py:   "ab" * 3
来源：http://byn.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://vbk.zhijiandao.cn

JS:   "ab".repeat(3)
来源：http://mpj.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://ayf.yuxming.cn

Java: "ab".repeat(3)
来源：http://iib.pycfn.com

Go:   strings.Repeat("ab", 3)
来源：http://rcy.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://wpv.guowangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bqj.nanxuanxn.top

[E03] 截取子串
来源：http://ygu.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ads.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://znh.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cas.birdmap.top

TS:   s.slice(1, 4)
来源：http://mij.havefunace.top

Java: s.substring(1, 4)
来源：http://too.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ulc.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://tij.shangyingyoupin.top

C#:   s.Substring(1, 3)
来源：http://say.pycfn.com

[E04] 查找子串位置
来源：http://bmz.shanyushiyangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://zgs.zhijiandao.cn

PHP:  strpos($s, "x");
来源：http://fuj.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tmb.aibaodan.cn

TS:   s.indexOf("x")
来源：http://edt.tianlin.xyz

Java: s.indexOf("x")
来源：http://ngn.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://vxs.9152youxi.cn

Ruby: s.index("x")
来源：http://fhx.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://dxr.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://nrc.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ein.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://thr.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fao.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kma.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nos.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ruc.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ucq.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zml.nanxuanxn.top

[E06] 替换子串
来源：http://lzg.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://skg.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://hfo.shanyushiyangtech.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://guu.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://grv.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wdl.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xla.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kla.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://sir.316326.xyz

[E07] 按分隔符拆分
来源：http://uiv.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://exu.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xbg.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mxg.cashguo.top

TS:   s.split(",")
来源：http://pie.sysykeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://seb.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qkv.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://qhb.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nxc.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://yxe.tanke756.top

Py:   ",".join(items)
来源：http://veg.sweek.top

PHP:  implode(",", $items);
来源：http://sal.jinghuilouyu.cn

JS:   items.join(",")
来源：http://ypx.zycfv.cn

TS:   items.join(",")
来源：http://zyp.meibo888.top

Java: String.join(",", items)
来源：http://xiz.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://jju.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://yhe.daria6918.cn

C#:   string.Join(",", items)
来源：http://fba.xinyue.icu

[E09] 去除所有空白字符
来源：http://ryf.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bjc.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://okq.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://wfi.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://eqo.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://mwv.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://edg.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hds.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zqf.hnxiangtu.top

[E10] 左侧补零 / 定长填充
来源：http://yvy.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://poi.dianchejie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pky.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://ubu.svipenyu.cn

TS:   "7".padStart(3, "0")
来源：http://tef.hywenlv.cn

Java: String.format("%03d", 7)
来源：http://wyg.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://doh.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ivn.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://krj.ydjk.org.cn

[E11] 反转字符串
来源：http://ajt.sxryk.cn

Py:   s[::-1]
来源：http://mcp.meibo888.top

PHP:  strrev($s);
来源：http://did.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://nkh.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://nay.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wjq.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kyk.ivvv.top

Ruby: s.reverse
来源：http://xcc.shanyushiyangtech.top

C#:   new string(s.Reverse().ToArray())
来源：http://gij.yanxiufei.cn

[E12] 统计某字符出现次数
来源：http://zsh.bjfxy.top

Py:   s.count("a")
来源：http://wmp.shanyushiyangkeji.top

PHP:  substr_count($s, "a");
来源：http://kzj.sweek.top

JS:   s.split("a").length - 1
来源：http://pii.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://rdj.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zmw.shzxlz.cn

Go:   strings.Count(s, "a")
来源：http://hpe.hnqzz.top

Ruby: s.count("a")
来源：http://cky.9152youxi.cn

C#:   s.Count(c => c == 'a')
来源：http://pkq.xylfe.cn

[E13] 逐字符遍历
来源：http://uwn.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://huh.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qlo.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zlz.nwbrower.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vtn.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zcy.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yvf.jlsjyb.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oqe.yj20258888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vuo.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://rgm.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nch.wangdashe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tap.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://utd.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://huk.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qib.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://axe.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xuq.hesvh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jdv.snrcjt.cn

[E15] HTML 转义 / 反转义
来源：http://kjh.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ofn.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://auk.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zae.pengpengdd.cyou

TS:   // 同上，务必做 XSS 过滤
来源：http://idd.jinyuanbaomall.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tlt.yvedp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ili.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://chp.bjfxy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xmf.tianlin.xyz

[E16] 数字千分位
来源：http://lcx.wangdashe.top

Py:   f"{1234567:,}"
来源：http://npd.bjfxy.top

PHP:  number_format(1234567);
来源：http://jwc.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jry.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yaw.shanyushiyangtech.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fql.zhongyouzk.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gcr.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://suz.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://qfh.chenjidiqi.icu

[E17] 首字母大写
来源：http://bun.daria6918.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://stg.shangyingyoupin.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kyv.meibo888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wgb.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wna.sysykeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kpm.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ens.dashuyun.cn

Ruby: s.capitalize
来源：http://dnl.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bdh.svipenyu.cn

[E18] 模板占位符替换
来源：http://kae.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cwq.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lzk.gaohongyu789.top

JS:   tpl.replaceAll("{name}", name)
来源：http://knj.yuxming.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xit.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ddp.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ryc.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mtv.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lqo.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://hvw.shangyingyoupin.top

Py:   s.splitlines()
来源：http://dnl.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pzv.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://bgq.fehbvm.com

TS:   s.split(/\r?\n/)
来源：http://xse.kuanghao11.cn

Java: s.lines().toList()
来源：http://okm.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://poj.vqdsnc.cn

Ruby: s.lines
来源：http://kbx.sufxvd.cn

C#:   s.Split('\n')
来源：http://ivt.jianghu66.top

[E20] 判断字符串是否为空
来源：http://ybm.pycfn.com

Py:   if not s:
来源：http://tqf.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fei.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qwf.ivvv.top

TS:   if (s === "") {}
来源：http://wqj.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://pxr.bjfxy.top

Go:   if s == "" {}
来源：http://cpu.daria6918.cn

Ruby: if s.empty?
来源：http://vub.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zlq.9152youxi.cn

[E21] 超长截断加省略号
来源：http://vnw.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://klm.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kpj.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zfd.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vhs.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yzf.chenjidiqi.icu

Go:   // 按 rune 判断长度后截断
来源：http://hqw.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://glo.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aad.cucudq.cn

[E22] 字节长度与字符长度
来源：http://oem.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pyi.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vvm.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://usu.hnqzz.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yio.yuanzhike.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hhs.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jiq.316326.xyz

Ruby: s.bytesize;  s.length
来源：http://xgk.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xtf.quarkkingdee.top

================================================================================
来源：http://kwd.feifeiyinyue.top

F. 文件与目录
来源：http://nsp.hongshengwenyu.top

================================================================================
来源：http://ste.cdnleiting.top

[F01] 读取整个文件
来源：http://vjp.cdnleiting.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wta.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://gre.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fri.jinqigfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wvc.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tps.jinqigfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wqi.bjfxy.top

Ruby: File.read("a.txt")
来源：http://iyh.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://pjz.daxiang520.top

[F02] 逐行读取文件
来源：http://mlk.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qom.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ouz.yongpay.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ojr.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wke.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tzh.svipenyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pbd.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://voq.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://syn.9152youxi.cn

[F03] 写入文件（覆盖）
来源：http://sgm.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sqf.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://azu.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cef.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://svh.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://orr.hnqzz.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xsf.mhx1999.top

Ruby: File.write("a.txt", "hi")
来源：http://jqa.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qzf.xuetiantiany.cn

[F04] 追加写入文件
来源：http://jqc.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pne.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lit.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iod.bbcook.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sln.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tus.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jnj.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uew.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ilh.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://pjp.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hhu.redwolf501.top

PHP:  file_exists("a.txt");
来源：http://kdh.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://fac.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://juc.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eiy.tian-w.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cka.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://fux.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://qec.shanyushiyangtech.top

[F06] 删除文件
来源：http://dkx.kuanghao11.cn

Py:   os.remove("a.txt")
来源：http://mbl.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://eri.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://spg.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://qho.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bef.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://fcr.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://bpz.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://ydf.yanxiufei.cn

[F07] 创建目录（含多级）
来源：http://jcw.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cxn.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ynq.guowangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://alb.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://umq.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://liq.andypj.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qyi.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zqu.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bwm.zhiwuduotai.top

[F08] 遍历目录
来源：http://iuy.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bvl.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bva.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://nuf.hysaishi.cn

TS:   fs.readdirSync("dir")
来源：http://yxw.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uks.zhengqikj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cgx.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://krp.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://kxq.ywan-chungtsiang.top


<!-- 参考信息 -->