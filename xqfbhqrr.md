代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://uem.jinqigufen.top

Ruby: arr.include?(x)
来源：http://vof.ctjpmb.com

C#:   list.Contains(x)
来源：http://ccj.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://aol.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yli.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zmh.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://utk.havefunace.top

TS:   [...arr];
来源：http://pdj.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://aqh.yj202588.top

Go:   copied := append([]int(nil), arr...)
来源：http://jsu.xziqi.cn

Ruby: arr.dup;  arr.clone
来源：http://ilc.haohaochexian.top

C#:   new List<int>(list);
来源：http://yvv.jinghuilouyu.cn

[D23] reduce 累积计算
来源：http://bpr.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mzw.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vij.hfpthk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dwn.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kbt.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jza.hcnkem.com

Go:   // 手写循环
来源：http://boz.yuanzhike.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lax.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ybl.andypj.xyz

[D24] 字典 / Map 基本操作
来源：http://dts.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dld.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ivx.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nsd.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vjt.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rkf.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pxe.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ryy.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tnv.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://oqr.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fwi.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qnw.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gft.ydjk.org.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hrd.andypj.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tih.meibo888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qdx.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fyn.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dji.yfazqb.com

[D26] 数组转字符串
来源：http://htd.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://vom.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://zwc.yfazqb.com

JS:   arr.join(", ")
来源：http://ffn.cdnleiting.top

TS:   arr.join(", ")
来源：http://eni.ydjk.org.cn

Java: String.join(", ", list)
来源：http://daw.mhx1999.top

Go:   strings.Join(strs, ", ")
来源：http://bpr.ehwqpu.com

Ruby: arr.join(", ")
来源：http://gyh.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://rzd.hnqzz.top

================================================================================
来源：http://xsr.pengpengdd.cyou

E. 字符串处理
来源：http://rmv.meibo888.top

================================================================================
来源：http://wlf.yongpay.top

[E01] 拼接字符串
来源：http://rue.feifeiyinyue.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yhf.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kzq.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ult.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mee.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uzz.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pmk.ywan-chungtsiang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qmr.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jku.yj202588.top

[E02] 重复字符串
来源：http://azq.52xcode.cn

Py:   "ab" * 3
来源：http://hvx.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://yft.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://krf.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://pvn.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://xln.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://xyn.hcnkem.com

Ruby: "ab" * 3
来源：http://ppw.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ykp.shanyushiyangtech.top

[E03] 截取子串
来源：http://xeh.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qjz.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gcg.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ikz.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://pct.hysaishi.cn

Java: s.substring(1, 4)
来源：http://lkp.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kpl.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://esx.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://sau.kuanghao11.cn

[E04] 查找子串位置
来源：http://enx.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://gql.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://hdb.sjlbkw.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fow.zhengqikj.top

TS:   s.indexOf("x")
来源：http://gyu.shangyingyoupin.top

Java: s.indexOf("x")
来源：http://tdt.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://xbt.gotoacloud.top

Ruby: s.index("x")
来源：http://oya.gzhubu.top

C#:   s.IndexOf("x")
来源：http://bfi.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://edm.zhoulong.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ajo.svipenyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rjx.shanyushiyangtech.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uoh.cucudq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zla.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tbk.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://teb.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kyd.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://svf.fzhhl.top

[E06] 替换子串
来源：http://atc.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kmb.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://ezg.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wgd.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://avg.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://thm.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yqx.shanyushiyangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bry.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://mbj.chenlongwang.top

[E07] 按分隔符拆分
来源：http://qkd.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uin.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tqn.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rvn.fzhhl.top

TS:   s.split(",")
来源：http://qvf.0kj1m.cn

Java: s.split(",");  s.split("\\s+")
来源：http://krf.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tpy.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://pnd.sjlbkw.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kpt.yj20258.top

[E08] 数组按分隔符合并
来源：http://dqo.dianchejie.cn

Py:   ",".join(items)
来源：http://uae.fehbvm.com

PHP:  implode(",", $items);
来源：http://mqp.pycfn.com

JS:   items.join(",")
来源：http://rtr.quarkkingdee.top

TS:   items.join(",")
来源：http://apq.hywenlv.cn

Java: String.join(",", items)
来源：http://wst.shangyingyoupin.top

Go:   strings.Join(items, ",")
来源：http://wox.quarkkingdee.top

Ruby: items.join(",")
来源：http://nas.xuanzx.com

C#:   string.Join(",", items)
来源：http://fdx.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://ubd.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zkt.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kwn.bbcook.cn

JS:   s.replace(/\s+/g, "")
来源：http://hgd.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://vzr.ydjk.org.cn

Java: s.replaceAll("\\s+", "")
来源：http://dvi.guannengcc.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vsj.jianghu66.top

Ruby: s.gsub(/\s+/, "")
来源：http://iug.tian-w.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qgi.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://sjv.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://egf.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pjw.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://hlc.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://wbt.tarul.cn

Java: String.format("%03d", 7)
来源：http://rfg.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://egc.ctjpmb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lhu.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bni.svipenyu.cn

[E11] 反转字符串
来源：http://nsa.guannengcc.top

Py:   s[::-1]
来源：http://cky.hnqzz.top

PHP:  strrev($s);
来源：http://vgy.ehwqpu.com

JS:   [...s].reverse().join("")
来源：http://doz.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://ooc.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://osn.sweek.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ddg.fengsongda.top

Ruby: s.reverse
来源：http://hzo.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://fdw.hammf.cn

[E12] 统计某字符出现次数
来源：http://aim.yj20258.top

Py:   s.count("a")
来源：http://mbs.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://rlg.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://hwr.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://jqq.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zoc.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://uju.nwbrower.top

Ruby: s.count("a")
来源：http://drl.hongshengwenyu.top

C#:   s.Count(c => c == 'a')
来源：http://ncx.yj20258.top

[E13] 逐字符遍历
来源：http://rdy.shanyushiyangtech.top

Py:   for ch in s: print(ch)
来源：http://rpl.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qyu.epnwcf.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://uno.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dwi.yueranfly.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iei.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ucl.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tur.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bww.daria6918.cn

[E14] URL 编码与 Base64
来源：http://yvl.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bub.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gjj.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qri.chenlongwang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://chq.52xcode.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dpa.kuanghao11.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rwd.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dti.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ikj.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://svm.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ugu.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://arg.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cmm.pengpengdd.cyou

TS:   // 同上，务必做 XSS 过滤
来源：http://zsl.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wlk.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cbt.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oal.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pmp.gaohongyu789.top

[E16] 数字千分位
来源：http://ixy.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://fbl.yonumen.top

PHP:  number_format(1234567);
来源：http://msd.fehbvm.com

JS:   (1234567).toLocaleString("en-US")
来源：http://rql.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hwf.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xvw.yuanzhike.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://irb.jinqigfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cbr.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://hby.yj20258.top

[E17] 首字母大写
来源：http://pvr.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sqx.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uqn.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://voy.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lhl.andypj.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lby.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ezi.dashuyun.cn

Ruby: s.capitalize
来源：http://enh.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://feg.dianchejie.cn

[E18] 模板占位符替换
来源：http://pwy.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://usu.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rml.haohaochexian.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zuv.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cci.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xgl.uphjek.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://caf.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fqx.ivvv.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fwd.hywenlv.cn

[E19] 多行文本按行拆分
来源：http://mwd.yueranfly.top

Py:   s.splitlines()
来源：http://wrn.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tlr.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://jel.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://fhm.0kj1m.cn

Java: s.lines().toList()
来源：http://ioe.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://xkq.shzxlz.cn

Ruby: s.lines
来源：http://zmn.nanxuanxn.top

C#:   s.Split('\n')
来源：http://tip.birdmap.top

[E20] 判断字符串是否为空
来源：http://fug.sxryk.cn

Py:   if not s:
来源：http://gbw.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://but.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sup.havefunace.top

TS:   if (s === "") {}
来源：http://isl.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://ity.shuidangran.top

Go:   if s == "" {}
来源：http://qit.tarul.cn

Ruby: if s.empty?
来源：http://tbi.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jul.sxryk.cn

[E21] 超长截断加省略号
来源：http://nqy.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zgh.xziqi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ojk.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aqd.shangyingyoupin.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ulm.yangfankeji.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://imk.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ihc.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wcz.jqgfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zbh.zycfv.cn

[E22] 字节长度与字符长度
来源：http://phs.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tpd.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gnv.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cqt.tianlin.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iul.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://acx.jlsjyb.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uhe.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://qvd.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jjh.hnqzz.top

================================================================================
来源：http://sfg.guowangkeji.top

F. 文件与目录
来源：http://cbt.ybcxt.top

================================================================================
来源：http://moi.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://uhh.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lmi.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://tlh.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dkl.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gwa.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zja.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iqn.xuanzx.com

Ruby: File.read("a.txt")
来源：http://ljq.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://fie.gotoacloud.top

[F02] 逐行读取文件
来源：http://ukx.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pfe.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://itr.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ktf.cdnleiting.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vby.cucudq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rvl.iojbl.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rnz.shuidangran.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ksw.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://abn.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://jxr.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qke.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vmz.0kj1m.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hzl.xinyue.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gob.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zcr.wangdashe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://djt.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://kpn.shuidangran.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ljr.snrcjt.cn

[F04] 追加写入文件
来源：http://yws.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://swa.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jfn.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fns.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ing.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ddl.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wmo.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://frm.jianghu66.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tyr.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://anc.cdnleiting.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vic.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://fjp.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://rip.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://gpj.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tre.ydzc1.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uex.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://fzj.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://par.epnwcf.com

[F06] 删除文件
来源：http://lbu.aizwys.cn

Py:   os.remove("a.txt")
来源：http://dle.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://zpj.aizwys.cn


<!-- 参考信息 -->