代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tic.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://sxq.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cku.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ktm.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jkp.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ygd.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aix.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aph.jinghuilouyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://esn.vehdjk.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qsc.guowangkeji.top

[D25] Set 集合去重与交并差
来源：http://zgc.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jth.hcnkem.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xif.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://akw.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gfc.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lcj.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oug.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://khf.vehdjk.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mws.zdqjudy.top

[D26] 数组转字符串
来源：http://kzf.ydzc1.top

Py:   ", ".join(map(str, arr))
来源：http://jvh.ivvv.top

PHP:  implode(", ", $arr);
来源：http://bzx.daria6918.cn

JS:   arr.join(", ")
来源：http://wdf.fehbvm.com

TS:   arr.join(", ")
来源：http://kmg.nanxinkj.top

Java: String.join(", ", list)
来源：http://luu.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://lqf.ppjwa.cn

Ruby: arr.join(", ")
来源：http://lyt.0kj1m.cn

C#:   string.Join(", ", list)
来源：http://ind.tian-w.cn

================================================================================
来源：http://vrd.jqgfzy.top

E. 字符串处理
来源：http://swl.haohaochexian.top

================================================================================
来源：http://yih.ehwqpu.com

[E01] 拼接字符串
来源：http://aih.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eks.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://epm.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qfx.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ogg.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dux.wangshuangyany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yll.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://soy.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gtv.tanke756.top

[E02] 重复字符串
来源：http://jlq.nanxuanxn.top

Py:   "ab" * 3
来源：http://jsk.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://grm.zhengqikj.top

JS:   "ab".repeat(3)
来源：http://jgq.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://sgx.cashguo.top

Java: "ab".repeat(3)
来源：http://mlb.zhengqikj.top

Go:   strings.Repeat("ab", 3)
来源：http://gmx.ydzc1.top

Ruby: "ab" * 3
来源：http://smv.zhiwuduotai.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yvp.dianchejie.cn

[E03] 截取子串
来源：http://yko.hnqzz.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hac.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uzi.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oxu.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://ggf.haohaochexian.top

Java: s.substring(1, 4)
来源：http://aqg.aizwys.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://itq.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://tiv.jianghu66.top

C#:   s.Substring(1, 3)
来源：http://vml.ydzc1.top

[E04] 查找子串位置
来源：http://eoc.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://uyv.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://jbp.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mum.yj20258.top

TS:   s.indexOf("x")
来源：http://xfj.chenlongwang.top

Java: s.indexOf("x")
来源：http://lmg.ppjwa.cn

Go:   strings.Index(s, "x")
来源：http://eyy.52xcode.cn

Ruby: s.index("x")
来源：http://fct.aizwys.cn

C#:   s.IndexOf("x")
来源：http://lwv.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zha.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://etd.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://reu.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dme.cashguo.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rxo.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jky.guannengcc.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://whw.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wer.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vzn.quarkkingdee.top

[E06] 替换子串
来源：http://bcj.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://enm.shanyushiyangtech.top

PHP:  str_replace("a", "b", $s);
来源：http://ugy.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bkv.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://zwd.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://adq.vqdsnc.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wzr.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xky.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://psi.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://vok.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rwq.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jkx.pengpengdd.cyou

JS:   s.split(",");  s.split(/\s+/)
来源：http://pfh.pengpengdd.cyou

TS:   s.split(",")
来源：http://eok.jinghuilouyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wvu.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://evv.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://rjf.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uot.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://nse.yueranfly.top

Py:   ",".join(items)
来源：http://xog.bjfxy.top

PHP:  implode(",", $items);
来源：http://nfn.aibaodan.cn

JS:   items.join(",")
来源：http://xfw.iojbl.cn

TS:   items.join(",")
来源：http://vmx.ybcxt.top

Java: String.join(",", items)
来源：http://jue.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://agm.yongpay.top

Ruby: items.join(",")
来源：http://bkv.chenlongwang.top

C#:   string.Join(",", items)
来源：http://wsa.gotoacloud.top

[E09] 去除所有空白字符
来源：http://kek.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ldf.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xzn.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://myw.jinqigfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://xqo.gotoacloud.top

Java: s.replaceAll("\\s+", "")
来源：http://olz.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://srm.cqqwz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rsu.fengsongda.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mpu.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://rkz.tian-w.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ljw.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dge.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://kmy.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://tbw.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://grk.yj20258.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qko.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jsm.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://czg.yvedp.cn

[E11] 反转字符串
来源：http://ftd.ivvv.top

Py:   s[::-1]
来源：http://jmb.sjlbkw.cn

PHP:  strrev($s);
来源：http://myb.guannengcc.top

JS:   [...s].reverse().join("")
来源：http://siw.zycfv.cn

TS:   [...s].reverse().join("")
来源：http://uff.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://vsi.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hpk.uphjek.com

Ruby: s.reverse
来源：http://rld.bjfxy.top

C#:   new string(s.Reverse().ToArray())
来源：http://ckn.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://xpa.jinqigfzy.top

Py:   s.count("a")
来源：http://ihw.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://hbe.shuidangran.top

JS:   s.split("a").length - 1
来源：http://krk.hnqzz.top

TS:   s.split("a").length - 1
来源：http://gxl.bbcook.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aih.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://hyp.ppjwa.cn

Ruby: s.count("a")
来源：http://uel.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://qkl.ctjpmb.com

[E13] 逐字符遍历
来源：http://wtk.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://kpo.pycfn.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jwi.iojbl.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ceh.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://uap.shanyushiyangtech.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lov.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mxw.wangdashe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ppx.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rel.gotoacloud.top

[E14] URL 编码与 Base64
来源：http://stt.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://twn.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gaf.hcnkem.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rcm.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zql.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ejg.wangshuangyany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uwz.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://txk.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kpr.shanyushiyangtech.top

[E15] HTML 转义 / 反转义
来源：http://mgh.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zaa.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tfj.wangdashe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ttn.yj202588.top

TS:   // 同上，务必做 XSS 过滤
来源：http://byz.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://adh.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hbk.yvedp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://srh.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kvj.feifeiyinyue.top

[E16] 数字千分位
来源：http://ucb.yj20258888.top

Py:   f"{1234567:,}"
来源：http://lmo.bjfxy.top

PHP:  number_format(1234567);
来源：http://erg.ydzc1.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dqe.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ktt.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zuo.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://szg.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jta.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://bvf.wangdashe.top

[E17] 首字母大写
来源：http://tiq.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nzd.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://app.yongpay.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ypb.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hpl.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wuf.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bpb.yj20258.top

Ruby: s.capitalize
来源：http://cgf.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wqd.yonumen.top

[E18] 模板占位符替换
来源：http://ard.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hwe.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xlq.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zio.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nqe.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://okx.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vsu.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ngh.ybcxt.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vmc.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://lou.jiagoushi.top

Py:   s.splitlines()
来源：http://fwg.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cqe.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://ief.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://xao.xuanzx.com

Java: s.lines().toList()
来源：http://ifg.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://dts.sxryk.cn

Ruby: s.lines
来源：http://yuq.hongshengwenyu.top

C#:   s.Split('\n')
来源：http://hnt.shangyingyoupin.top

[E20] 判断字符串是否为空
来源：http://qdm.vqdsnc.cn

Py:   if not s:
来源：http://hqu.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://esl.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tlc.zhixingplan.top

TS:   if (s === "") {}
来源：http://jvk.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://nrl.yfazqb.com

Go:   if s == "" {}
来源：http://zkt.feifeiyinyue.top

Ruby: if s.empty?
来源：http://zoz.zdbjq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bjj.tian-w.cn

[E21] 超长截断加省略号
来源：http://kde.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://anx.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bzn.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ijf.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rrl.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uoa.shanyushiyangtech.top

Go:   // 按 rune 判断长度后截断
来源：http://eap.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kqr.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ymb.jinyuanbaomall.cn

[E22] 字节长度与字符长度
来源：http://tkd.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wur.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cct.andypj.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nbo.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tdp.jianghu66.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://msa.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xxk.9152youxi.cn

Ruby: s.bytesize;  s.length
来源：http://ehh.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nnv.sufxvd.cn

================================================================================
来源：http://cai.chenjidiqi.icu

F. 文件与目录
来源：http://qem.zhongyouzk.top

================================================================================
来源：http://cyx.jyoumei.cn

[F01] 读取整个文件
来源：http://pib.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nyh.hcnkem.com

PHP:  file_get_contents("a.txt");
来源：http://lqp.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rux.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://aqx.ydzc1.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xge.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://prp.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://oyp.fengsongda.top

C#:   File.ReadAllText("a.txt");
来源：http://kfp.epnwcf.com

[F02] 逐行读取文件
来源：http://wuk.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://obg.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ipe.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bye.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oaj.gogol.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jba.jinghuilouyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vtm.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fxu.cucudq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wuf.sjlbkw.cn

[F03] 写入文件（覆盖）
来源：http://twu.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lyl.cdnleiting.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dud.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sds.52xcode.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qkb.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vfm.chenlongwang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kpv.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://ncs.haohaochexian.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vhp.jyoumei.cn

[F04] 追加写入文件
来源：http://cmf.jinghuilouyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zvz.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pwo.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lbh.xinyue.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ptx.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sgl.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rrr.hnqzz.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zqi.chenlongwang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sxb.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://upz.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hmg.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://vlu.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://rxj.zdbjq.cn

TS:   fs.existsSync("a.txt")
来源：http://zrl.hnxiangtu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ojq.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://etp.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://pai.meibo888.top

C#:   File.Exists("a.txt")
来源：http://gok.havefunace.top

[F06] 删除文件
来源：http://vhm.52xcode.cn

Py:   os.remove("a.txt")
来源：http://yzt.yuanzhike.top

PHP:  unlink("a.txt");
来源：http://uwm.nanxinkj.top

JS:   fs.unlinkSync("a.txt")
来源：http://dho.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://rua.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dcv.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://jzj.sweek.top

Ruby: File.delete("a.txt")
来源：http://cqv.birdmap.top

C#:   File.Delete("a.txt");
来源：http://qit.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://cqp.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yzb.shanyushiyangtech.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xfx.jianghu66.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://svb.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vpt.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pzp.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dkz.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mwe.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fzl.zdqjudy.top

[F08] 遍历目录
来源：http://nqm.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jsf.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rhr.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://qdb.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://ccv.zhoulong.xyz


<!-- 参考信息 -->