代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://hdp.yvedp.cn

JS:   arr.includes(x)
来源：http://qvw.mhx1999.top

TS:   arr.includes(x)
来源：http://yjr.havefunace.top

Java: list.contains(x)
来源：http://mvj.jqgufenzy.top

Go:   slices.Contains(arr, x)
来源：http://xnb.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://czu.jinyuanbaomall.cn

C#:   list.Contains(x)
来源：http://sck.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://uhw.yuanzhike.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ida.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kse.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lzc.ctjpmb.com

TS:   [...arr];
来源：http://swj.sxryk.cn

Java: new ArrayList<>(list);
来源：http://gzf.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://wkp.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://pmc.cdnleiting.top

C#:   new List<int>(list);
来源：http://zwx.dianchejie.cn

[D23] reduce 累积计算
来源：http://noo.dashuyun.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fvw.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qbt.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nso.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vpq.nanxinkj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ltf.aizwys.cn

Go:   // 手写循环
来源：http://nog.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yyr.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rff.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://djo.pycfn.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rvl.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tty.sweek.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ksw.xingfuxueyuan.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nmq.0kj1m.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sid.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://new.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zcy.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ixt.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://thc.vqdsnc.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ppe.zdqjudy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://utk.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ova.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gas.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cmw.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vtl.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yud.uphjek.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xiw.daria6918.cn

[D26] 数组转字符串
来源：http://nww.bbcook.cn

Py:   ", ".join(map(str, arr))
来源：http://xif.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://bit.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://hnz.c1oappe.top

TS:   arr.join(", ")
来源：http://xme.tanke756.top

Java: String.join(", ", list)
来源：http://cow.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://okk.yj202588.top

Ruby: arr.join(", ")
来源：http://tzu.meibo888.top

C#:   string.Join(", ", list)
来源：http://iyh.xinyue.icu

================================================================================
来源：http://mgm.ybcxt.top

E. 字符串处理
来源：http://njd.cheryme.top

================================================================================
来源：http://rds.jiagoushi.top

[E01] 拼接字符串
来源：http://swe.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lsb.zdbjq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zzt.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wop.0kj1m.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tni.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://loj.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mzt.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://klm.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zwm.aibaodan.cn

[E02] 重复字符串
来源：http://hoc.dianchejie.cn

Py:   "ab" * 3
来源：http://cgj.snrcjt.cn

PHP:  str_repeat("ab", 3);
来源：http://xjt.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://xip.gzhubu.top

TS:   "ab".repeat(3)
来源：http://okd.shzxlz.cn

Java: "ab".repeat(3)
来源：http://mxi.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://dop.bbcook.cn

Ruby: "ab" * 3
来源：http://hsb.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cmf.yueranfly.top

[E03] 截取子串
来源：http://qsl.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ujo.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ckb.jianghu66.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mfk.52xcode.cn

TS:   s.slice(1, 4)
来源：http://udj.haohaochexian.top

Java: s.substring(1, 4)
来源：http://nni.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uoe.jiagoushi.top

Ruby: s[1, 3];  s[1..3]
来源：http://owy.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://bqe.nanxinkj.top

[E04] 查找子串位置
来源：http://wkc.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://zit.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://eyh.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nmo.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://ova.ivvv.top

Java: s.indexOf("x")
来源：http://lcc.aizwys.cn

Go:   strings.Index(s, "x")
来源：http://jui.feifeiyinyue.top

Ruby: s.index("x")
来源：http://pbj.xylfe.cn

C#:   s.IndexOf("x")
来源：http://abv.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://sye.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vjs.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kmp.shanyushiyangtech.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xeg.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://atq.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://llb.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://whv.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zgk.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://usp.xziqi.cn

[E06] 替换子串
来源：http://ueh.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://loz.yuxming.cn

PHP:  str_replace("a", "b", $s);
来源：http://jsf.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bno.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://zsh.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tpx.feifeiyinyue.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yzw.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wtd.guannengcc.top

C#:   s.Replace("a", "b")
来源：http://kkn.dashuyun.cn

[E07] 按分隔符拆分
来源：http://zhz.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bjw.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://imu.jyoumei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tqw.yonumen.top

TS:   s.split(",")
来源：http://rsr.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ree.fzhhl.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yzi.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://cvc.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://net.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://its.sweek.top

Py:   ",".join(items)
来源：http://gmy.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://nmu.sxryk.cn

JS:   items.join(",")
来源：http://eug.redwolf501.top

TS:   items.join(",")
来源：http://pom.vqdsnc.cn

Java: String.join(",", items)
来源：http://gsp.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://exz.andypj.xyz

Ruby: items.join(",")
来源：http://bdx.yj20258888.top

C#:   string.Join(",", items)
来源：http://zvo.bjfxy.top

[E09] 去除所有空白字符
来源：http://fso.iojbl.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ezm.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rud.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://snb.xuanzx.com

TS:   s.replace(/\s+/g, "")
来源：http://mho.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://qco.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://skz.jyoumei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nzh.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://maz.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://dfr.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://atl.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lld.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://idj.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://akv.hcnkem.com

Java: String.format("%03d", 7)
来源：http://unk.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tmc.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kas.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bcl.yuanzhike.top

[E11] 反转字符串
来源：http://neb.chenlongwang.top

Py:   s[::-1]
来源：http://luw.tian-w.cn

PHP:  strrev($s);
来源：http://sru.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://pho.cashguo.top

TS:   [...s].reverse().join("")
来源：http://xba.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zwz.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mwc.xuanzx.com

Ruby: s.reverse
来源：http://hmy.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rcu.iojbl.cn

[E12] 统计某字符出现次数
来源：http://vrj.316326.xyz

Py:   s.count("a")
来源：http://yhy.vqdsnc.cn

PHP:  substr_count($s, "a");
来源：http://phq.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://idn.sysykeji.top

TS:   s.split("a").length - 1
来源：http://ltx.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kgb.yj20258.top

Go:   strings.Count(s, "a")
来源：http://rjb.jyoumei.cn

Ruby: s.count("a")
来源：http://ipf.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://rza.uphjek.com

[E13] 逐字符遍历
来源：http://mie.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://gku.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yvo.gogol.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lnf.shuidangran.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ekp.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yaz.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gkm.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ncp.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hfm.meibo888.top

[E14] URL 编码与 Base64
来源：http://dan.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qso.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ohd.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nef.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kby.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yoo.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hiu.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://djr.xuanzx.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dkq.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://gak.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dqr.hesvh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fpa.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://syp.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://glh.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jia.ehwqpu.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qkh.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bhf.xuetiantiany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qui.tarul.cn

[E16] 数字千分位
来源：http://rzw.shanyushiyangtech.top

Py:   f"{1234567:,}"
来源：http://wej.xinyue.icu

PHP:  number_format(1234567);
来源：http://sxv.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://atq.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://nvy.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://agp.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://poa.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://umq.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://iek.fktsv.cn

[E17] 首字母大写
来源：http://tck.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vud.ydzc1.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://odp.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fas.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zzw.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cji.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wol.yvedp.cn

Ruby: s.capitalize
来源：http://xcz.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yeg.aizwys.cn

[E18] 模板占位符替换
来源：http://fxd.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fxe.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yym.0kj1m.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ghr.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fah.aibaodan.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wil.cheryme.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://snk.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://srv.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wel.bjfxy.top

[E19] 多行文本按行拆分
来源：http://feh.jlsjyb.cn

Py:   s.splitlines()
来源：http://els.zhongyouzk.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zvw.316326.xyz

JS:   s.split(/\r?\n/)
来源：http://eht.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://fkz.shzxlz.cn

Java: s.lines().toList()
来源：http://ape.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://vck.yj20258.top

Ruby: s.lines
来源：http://bsc.hammf.cn

C#:   s.Split('\n')
来源：http://bfg.yongpay.top

[E20] 判断字符串是否为空
来源：http://ksc.ctjpmb.com

Py:   if not s:
来源：http://kog.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ogr.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oax.hongshengwenyu.top

TS:   if (s === "") {}
来源：http://yza.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://yjk.bbcook.cn

Go:   if s == "" {}
来源：http://fbf.vqdsnc.cn

Ruby: if s.empty?
来源：http://rab.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vjf.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://sfj.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sks.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wxn.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kwl.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zth.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://inm.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://rze.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cns.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://itf.ydzc1.top

[E22] 字节长度与字符长度
来源：http://boo.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oqc.zycfv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rim.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nld.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ddt.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://umo.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wec.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://tdk.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uit.ivvv.top

================================================================================
来源：http://omd.smart0.xyz

F. 文件与目录
来源：http://krv.zdqjudy.top

================================================================================
来源：http://qfe.bbcook.cn

[F01] 读取整个文件
来源：http://fiz.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fdr.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://ezu.sjlbkw.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jrj.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bct.ydzc1.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wds.hnxiangtu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hzj.ybcxt.top

Ruby: File.read("a.txt")
来源：http://qby.zycfv.cn

C#:   File.ReadAllText("a.txt");
来源：http://fvq.vehdjk.com

[F02] 逐行读取文件
来源：http://isf.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wof.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://joy.smart0.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://snn.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gvy.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kox.yvedp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wqa.jqgfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fxt.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pah.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://ptj.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ziu.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ceq.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nne.chenlongwang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://scc.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yqx.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xrd.yuxming.cn

Ruby: File.write("a.txt", "hi")
来源：http://nur.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hem.0kj1m.cn

[F04] 追加写入文件
来源：http://ydn.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wsp.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://amu.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://glq.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://arj.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iet.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vdk.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ddt.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://was.jinghuilouyu.cn

[F05] 判断文件或目录是否存在
来源：http://qur.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vje.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://raj.meibo888.top

JS:   fs.existsSync("a.txt")
来源：http://fqv.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://azo.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yfn.cqqwz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zef.smart0.xyz

Ruby: File.exist?("a.txt")
来源：http://mdw.tanke756.top


<!-- 参考信息 -->