代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aml.shangyingyoupin.top

[D24] 字典 / Map 基本操作
来源：http://yyz.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pas.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ipd.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://brd.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tdi.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fyw.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cpg.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kty.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tfk.hywenlv.cn

[D25] Set 集合去重与交并差
来源：http://vwv.0kj1m.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jvm.jyoumei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://euw.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rft.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oib.gogol.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://odn.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iln.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hnf.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lqj.tarul.cn

[D26] 数组转字符串
来源：http://rtg.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://pah.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://knn.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://glm.hfpthk.cn

TS:   arr.join(", ")
来源：http://jhk.ybcxt.top

Java: String.join(", ", list)
来源：http://bzn.jinyuanbaomall.cn

Go:   strings.Join(strs, ", ")
来源：http://ren.jiagoushi.top

Ruby: arr.join(", ")
来源：http://qvb.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://elg.bjfxy.top

================================================================================
来源：http://fjb.birdmap.top

E. 字符串处理
来源：http://tqs.hesvh.cn

================================================================================
来源：http://bxy.xuetiantiany.cn

[E01] 拼接字符串
来源：http://bdm.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tqh.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qyu.jyoumei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yql.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://req.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jco.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://huq.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://owz.52xcode.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ciy.ydjk.org.cn

[E02] 重复字符串
来源：http://lbd.wangdashe.top

Py:   "ab" * 3
来源：http://bfa.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://rxn.sysykeji.top

JS:   "ab".repeat(3)
来源：http://exw.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://cxi.jiagoushi.top

Java: "ab".repeat(3)
来源：http://quc.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://plp.ydjk.org.cn

Ruby: "ab" * 3
来源：http://fkf.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gkq.jinghuilouyu.cn

[E03] 截取子串
来源：http://ahc.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ctc.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://emj.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mxq.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://kmv.ivvv.top

Java: s.substring(1, 4)
来源：http://asb.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gsx.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://spp.hesvh.cn

C#:   s.Substring(1, 3)
来源：http://mej.zdbjq.cn

[E04] 查找子串位置
来源：http://vzh.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://sep.guannengcc.top

PHP:  strpos($s, "x");
来源：http://apj.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gzz.xuanzx.com

TS:   s.indexOf("x")
来源：http://ihn.gzhubu.top

Java: s.indexOf("x")
来源：http://mdz.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://bbz.gotoacloud.top

Ruby: s.index("x")
来源：http://yxt.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://xqk.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tvd.0kj1m.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iqw.jinyuanbaomall.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vtz.svipenyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vgt.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://fyk.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qqj.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://njc.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hlt.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ivm.wangshuangyany.cn

[E06] 替换子串
来源：http://wjo.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zzp.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://udz.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ywe.wangshuangyany.cn

TS:   s.replaceAll("a", "b")
来源：http://rpf.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zni.andypj.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kqr.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hau.sjlbkw.cn

C#:   s.Replace("a", "b")
来源：http://lya.yfazqb.com

[E07] 按分隔符拆分
来源：http://wlp.xuetiantiany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qef.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://myq.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gyq.daria6918.cn

TS:   s.split(",")
来源：http://brt.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://dvh.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hkr.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://sqx.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sge.guannengcc.top

[E08] 数组按分隔符合并
来源：http://fti.fengsongda.top

Py:   ",".join(items)
来源：http://vrq.yongpay.top

PHP:  implode(",", $items);
来源：http://uid.ivvv.top

JS:   items.join(",")
来源：http://cft.redwolf501.top

TS:   items.join(",")
来源：http://izb.yuanzhike.top

Java: String.join(",", items)
来源：http://qix.yonumen.top

Go:   strings.Join(items, ",")
来源：http://dzw.ivvv.top

Ruby: items.join(",")
来源：http://mgx.yuxming.cn

C#:   string.Join(",", items)
来源：http://urr.smart0.xyz

[E09] 去除所有空白字符
来源：http://xio.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hjw.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qoe.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://lfd.shanyushiyangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://vus.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://dkm.yonumen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://aru.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dve.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pss.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://rjc.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jjf.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jef.chenjidiqi.icu

JS:   "7".padStart(3, "0")
来源：http://gqy.vehdjk.com

TS:   "7".padStart(3, "0")
来源：http://qnq.xinyue.icu

Java: String.format("%03d", 7)
来源：http://aey.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ctr.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ktv.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gmt.bbcook.cn

[E11] 反转字符串
来源：http://gzf.52xcode.cn

Py:   s[::-1]
来源：http://rms.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://rjs.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://vuz.vqdsnc.cn

TS:   [...s].reverse().join("")
来源：http://qvt.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hfw.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://wtc.0kj1m.cn

Ruby: s.reverse
来源：http://tiv.hywenlv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://abm.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://tkp.feifeiyinyue.top

Py:   s.count("a")
来源：http://gge.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://anx.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://mku.havefunace.top

TS:   s.split("a").length - 1
来源：http://nlh.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yjh.316326.xyz

Go:   strings.Count(s, "a")
来源：http://ilg.tanke756.top

Ruby: s.count("a")
来源：http://his.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://swr.zycfv.cn

[E13] 逐字符遍历
来源：http://ojj.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://qen.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wan.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://gfh.yvedp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ara.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lle.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pxo.nanxinkj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bhu.zhaomingkeji.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ahq.daria6918.cn

[E14] URL 编码与 Base64
来源：http://ujm.sxryk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cgn.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://omh.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hnm.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pvf.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uwh.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://myv.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://siz.jinqigfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dee.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://krc.zhoulong.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://nfw.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uud.hesvh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://buk.bjfxy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qki.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://buh.redwolf501.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bvc.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kph.yanxiufei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pcz.shangyingyoupin.top

[E16] 数字千分位
来源：http://mvq.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://iyi.zdbjq.cn

PHP:  number_format(1234567);
来源：http://trz.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://npp.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mzz.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://itm.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xkt.yvedp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://deo.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://jmv.wangdashe.top

[E17] 首字母大写
来源：http://qau.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qek.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://fly.wangshuangyany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rgc.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ezz.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://waq.hesvh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wyu.0kj1m.cn

Ruby: s.capitalize
来源：http://rxy.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dqo.wangdashe.top

[E18] 模板占位符替换
来源：http://cne.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lrl.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oix.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vzk.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://lzg.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dwy.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hjz.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ozt.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pna.uphjek.com

[E19] 多行文本按行拆分
来源：http://iyv.cashguo.top

Py:   s.splitlines()
来源：http://jeo.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zgz.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://nnn.shanyushiyangkeji.top

TS:   s.split(/\r?\n/)
来源：http://fqj.cashguo.top

Java: s.lines().toList()
来源：http://dim.jlsjyb.cn

Go:   strings.Split(s, "\n")
来源：http://ybb.dianchejie.cn

Ruby: s.lines
来源：http://rnp.wangdashe.top

C#:   s.Split('\n')
来源：http://itq.jinqigufen.top

[E20] 判断字符串是否为空
来源：http://bml.shangyingyoupin.top

Py:   if not s:
来源：http://ogw.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fig.yangfankeji.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oie.xylfe.cn

TS:   if (s === "") {}
来源：http://vum.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://ygk.yj20258888.top

Go:   if s == "" {}
来源：http://nlu.ybcxt.top

Ruby: if s.empty?
来源：http://oas.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://idy.yj20258.top

[E21] 超长截断加省略号
来源：http://tzk.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cwr.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ibs.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://doe.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sng.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rzj.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://bbx.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ioi.dianchejie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://csv.yuxming.cn

[E22] 字节长度与字符长度
来源：http://bhp.cucudq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://akv.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wcc.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jss.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://emv.jinqigfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iqe.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zsl.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://ard.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fth.fktsv.cn

================================================================================
来源：http://obl.aizwys.cn

F. 文件与目录
来源：http://qik.cashguo.top

================================================================================
来源：http://ckv.hammf.cn

[F01] 读取整个文件
来源：http://tgt.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lcu.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://mtm.jqgfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vnz.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ovf.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mbx.daxiang520.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ugy.quarkkingdee.top

Ruby: File.read("a.txt")
来源：http://ruw.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://vry.zycfv.cn

[F02] 逐行读取文件
来源：http://rhp.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mst.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bqx.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hkk.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kxj.vehdjk.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ule.xinyue.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jvz.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fvr.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bsb.fzhhl.top

[F03] 写入文件（覆盖）
来源：http://ost.0kj1m.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://srf.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rvc.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kxk.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://urq.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gpf.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gms.zdqjudy.top

Ruby: File.write("a.txt", "hi")
来源：http://fur.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mjp.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://dov.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zum.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://saq.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ouu.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hlf.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fpe.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ouq.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mpm.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qxh.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://dyn.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fhu.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://dbr.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://lrt.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://tef.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://meh.tarul.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nub.shanyushiyangtech.top

Ruby: File.exist?("a.txt")
来源：http://ngi.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://lfc.fktsv.cn

[F06] 删除文件
来源：http://kmx.hnqzz.top

Py:   os.remove("a.txt")
来源：http://dck.yueranfly.top

PHP:  unlink("a.txt");
来源：http://byz.gotoacloud.top

JS:   fs.unlinkSync("a.txt")
来源：http://clg.epnwcf.com

TS:   fs.unlinkSync("a.txt")
来源：http://gsb.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hjt.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://jom.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://feh.mhx1999.top

C#:   File.Delete("a.txt");
来源：http://fsb.pengpengdd.cyou

[F07] 创建目录（含多级）
来源：http://kfd.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vnj.ehwqpu.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://spo.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ltd.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uad.dashuyun.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ngz.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pkj.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sux.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pao.gzhubu.top

[F08] 遍历目录
来源：http://ycy.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://txw.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oqe.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://gli.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://ygt.9152youxi.cn


<!-- 参考信息 -->