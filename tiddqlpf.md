代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xcl.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://qvf.fanxiaobao.xyz

Go:   // 手写循环
来源：http://ksf.zycfv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hne.sweek.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lpe.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://jbd.birdmap.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vku.zhoulong.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oci.sufxvd.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sqk.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xxd.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://byf.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zvd.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://exc.snrcjt.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jwm.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://pxw.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fpx.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ucg.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fbn.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uxt.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ewi.hysaishi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mgo.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pes.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kuv.sysykeji.top

[D26] 数组转字符串
来源：http://mxs.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://jwy.52xcode.cn

PHP:  implode(", ", $arr);
来源：http://wnu.ehwqpu.com

JS:   arr.join(", ")
来源：http://ygv.quarkkingdee.top

TS:   arr.join(", ")
来源：http://dqz.guannengcc.top

Java: String.join(", ", list)
来源：http://eeb.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://xeu.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://leq.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://tsi.yj20258888.top

================================================================================
来源：http://iyw.yueranfly.top

E. 字符串处理
来源：http://bhp.feifeiyinyue.top

================================================================================
来源：http://jle.uphjek.com

[E01] 拼接字符串
来源：http://cov.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jbd.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mba.jqgfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qiz.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fnn.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pfz.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xzs.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ilr.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ayd.xuanzx.com

[E02] 重复字符串
来源：http://bgm.zhengqikj.top

Py:   "ab" * 3
来源：http://ias.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://ymq.hysaishi.cn

JS:   "ab".repeat(3)
来源：http://bdc.tanke756.top

TS:   "ab".repeat(3)
来源：http://wvf.yueranfly.top

Java: "ab".repeat(3)
来源：http://vys.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://wsn.0kj1m.cn

Ruby: "ab" * 3
来源：http://pmv.fehbvm.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iem.zycfv.cn

[E03] 截取子串
来源：http://qyl.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lsf.ybcxt.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dsj.yfazqb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yww.tarul.cn

TS:   s.slice(1, 4)
来源：http://jzf.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://ows.aizwys.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kdq.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://qig.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://sgr.ehwqpu.com

[E04] 查找子串位置
来源：http://tsj.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://ksi.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://nqh.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://owa.fanxiaobao.xyz

TS:   s.indexOf("x")
来源：http://wap.tarul.cn

Java: s.indexOf("x")
来源：http://qkl.xingfuxueyuan.xyz

Go:   strings.Index(s, "x")
来源：http://vku.gzhubu.top

Ruby: s.index("x")
来源：http://rzr.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://mdh.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xzo.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aes.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://emo.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dll.hammf.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://toh.shangyingyoupin.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ait.bjfxy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dko.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pme.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wlf.hfpthk.cn

[E06] 替换子串
来源：http://pea.zhongyouzk.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cuk.jinqigfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://tzu.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://btj.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://deg.hnxiangtu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dpc.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lvf.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ecn.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://rjy.snrcjt.cn

[E07] 按分隔符拆分
来源：http://rih.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fiu.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pnn.9152youxi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nad.yfazqb.com

TS:   s.split(",")
来源：http://tyl.gaohongyu789.top

Java: s.split(",");  s.split("\\s+")
来源：http://thm.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xlx.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://dzz.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bzp.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://ffs.ybcxt.top

Py:   ",".join(items)
来源：http://yhm.hesvh.cn

PHP:  implode(",", $items);
来源：http://ynq.bjfxy.top

JS:   items.join(",")
来源：http://okk.yongpay.top

TS:   items.join(",")
来源：http://wzl.jlsjyb.cn

Java: String.join(",", items)
来源：http://tcm.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://kix.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://caa.bbcook.cn

C#:   string.Join(",", items)
来源：http://muo.aizwys.cn

[E09] 去除所有空白字符
来源：http://htc.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jch.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zfg.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://jgy.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://pev.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://eyf.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fgm.jianghu66.top

Ruby: s.gsub(/\s+/, "")
来源：http://yob.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://efn.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://xgl.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qer.fehbvm.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://awc.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://rgz.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://xfa.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://jcv.svipenyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://itn.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lga.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sas.fzhhl.top

[E11] 反转字符串
来源：http://fnu.fanxiaobao.xyz

Py:   s[::-1]
来源：http://krx.ivvv.top

PHP:  strrev($s);
来源：http://rsy.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://sxb.yj20258888.top

TS:   [...s].reverse().join("")
来源：http://xwg.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tto.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pli.pycfn.com

Ruby: s.reverse
来源：http://umj.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://eqt.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://ili.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://fin.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://yzj.xylfe.cn

JS:   s.split("a").length - 1
来源：http://xiu.xylfe.cn

TS:   s.split("a").length - 1
来源：http://wbd.yangfankeji.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uqy.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://zhp.gzhubu.top

Ruby: s.count("a")
来源：http://wmz.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://zrr.jqgufenzy.top

[E13] 逐字符遍历
来源：http://lfx.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://fmb.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://idc.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://prk.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uss.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jkv.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wwi.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cec.ydjk.org.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kbx.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://fcl.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jzr.dianchejie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tbz.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vyz.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://krt.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://odr.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cmt.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ysr.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wli.hammf.cn

[E15] HTML 转义 / 反转义
来源：http://vdq.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pir.snrcjt.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://daz.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qxe.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mry.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mwm.fanxiaobao.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hsi.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://thk.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rbp.shanyushiyangtech.top

[E16] 数字千分位
来源：http://bea.yj20258.top

Py:   f"{1234567:,}"
来源：http://mml.chenlongwang.top

PHP:  number_format(1234567);
来源：http://urp.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://tol.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ijr.andypj.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qtv.zhijiandao.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://irp.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gqu.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://wgo.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://kfc.guowangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xta.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fcb.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pwz.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cqt.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xgr.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ddb.fehbvm.com

Ruby: s.capitalize
来源：http://lnv.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dhp.epnwcf.com

[E18] 模板占位符替换
来源：http://yav.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dnm.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zrn.yj20258.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zjm.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://idk.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ifv.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://idn.pengpengdd.cyou

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lba.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nrb.bjfxy.top

[E19] 多行文本按行拆分
来源：http://qxj.316326.xyz

Py:   s.splitlines()
来源：http://sly.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://val.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://dfb.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://nxs.havefunace.top

Java: s.lines().toList()
来源：http://rxu.yfazqb.com

Go:   strings.Split(s, "\n")
来源：http://vwx.fehbvm.com

Ruby: s.lines
来源：http://dng.meibo888.top

C#:   s.Split('\n')
来源：http://tdo.yuanzhike.top

[E20] 判断字符串是否为空
来源：http://zxn.hnqzz.top

Py:   if not s:
来源：http://zaq.nanxuanxn.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iwn.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fga.bbcook.cn

TS:   if (s === "") {}
来源：http://ldl.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://eqp.hesvh.cn

Go:   if s == "" {}
来源：http://ofj.ydjk.org.cn

Ruby: if s.empty?
来源：http://oya.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://piq.guowangkeji.top

[E21] 超长截断加省略号
来源：http://fqt.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qut.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kbn.fanxiaobao.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lom.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xyu.jlsjyb.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wra.zhengqikj.top

Go:   // 按 rune 判断长度后截断
来源：http://fpw.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lqh.shzxlz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://acq.yuxming.cn

[E22] 字节长度与字符长度
来源：http://ikm.tanke756.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vhl.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xox.yanxiufei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xtn.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ovn.shzxlz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ign.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pze.gzhubu.top

Ruby: s.bytesize;  s.length
来源：http://hmi.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://anu.hongshengwenyu.top

================================================================================
来源：http://rec.zhengqikj.top

F. 文件与目录
来源：http://bjp.wangdashe.top

================================================================================
来源：http://aem.kuanghao11.cn

[F01] 读取整个文件
来源：http://lji.ivvv.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ols.hywenlv.cn

PHP:  file_get_contents("a.txt");
来源：http://wlf.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rgd.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tcy.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ufv.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bsm.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://qgc.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://nmz.gogol.net.cn

[F02] 逐行读取文件
来源：http://gyd.ctjpmb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://man.sxryk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pxo.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xup.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lsp.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://olc.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://utr.ydzc1.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mwo.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://swt.xylfe.cn

[F03] 写入文件（覆盖）
来源：http://dfk.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fkh.fehbvm.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xjv.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vzg.chenlongwang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aux.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kos.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ezu.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://fhl.yj20258888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bvy.zycfv.cn

[F04] 追加写入文件
来源：http://gsy.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nux.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bil.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://whc.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oxa.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ony.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zkm.yanxiufei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kwo.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zrs.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://fyg.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zep.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://ydj.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://ujk.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://xsz.jyoumei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kwh.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://szp.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://wnm.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://dlm.fengsongda.top

[F06] 删除文件
来源：http://uwm.hammf.cn

Py:   os.remove("a.txt")
来源：http://mhv.hesvh.cn

PHP:  unlink("a.txt");
来源：http://vfi.svipenyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zat.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://nrg.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hiq.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://rgc.sweek.top

Ruby: File.delete("a.txt")
来源：http://vah.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://elh.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://znu.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jhb.snrcjt.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://usz.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zgv.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yyu.aibaodan.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cfs.yongpay.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://chw.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dio.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eeh.hysaishi.cn

[F08] 遍历目录
来源：http://atv.yfazqb.com


<!-- 参考信息 -->