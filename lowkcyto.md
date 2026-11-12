代发 wailian999

Ruby: arr.tally
来源：http://aeb.yuanzhike.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://avt.ydzc1.top

[D21] 判断是否包含某元素
来源：http://zmj.zhaomingkeji.xyz

Py:   x in arr
来源：http://tlx.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://qle.daria6918.cn

JS:   arr.includes(x)
来源：http://igp.shuidangran.top

TS:   arr.includes(x)
来源：http://pzf.zhongyouzk.top

Java: list.contains(x)
来源：http://jxf.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://fxe.yuxming.cn

Ruby: arr.include?(x)
来源：http://crq.9152youxi.cn

C#:   list.Contains(x)
来源：http://boq.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://xlw.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://owb.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ihr.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gpj.nwbrower.top

TS:   [...arr];
来源：http://bly.jyoumei.cn

Java: new ArrayList<>(list);
来源：http://rjr.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://adf.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://rik.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://uuv.jlsjyb.cn

[D23] reduce 累积计算
来源：http://ira.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xpv.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://krd.chenlongwang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://inm.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kyy.xylfe.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bkf.hesvh.cn

Go:   // 手写循环
来源：http://bkk.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rfg.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://egx.hesvh.cn

[D24] 字典 / Map 基本操作
来源：http://qeo.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hgi.nanxinkj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mfg.redwolf501.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pyy.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xcj.0kj1m.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lwv.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pnn.hywenlv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jhy.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wcj.pengpengdd.cyou

[D25] Set 集合去重与交并差
来源：http://ihc.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mvt.guannengcc.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://klr.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jqi.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iju.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pet.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nni.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dbm.hesvh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kdp.pycfn.com

[D26] 数组转字符串
来源：http://hqz.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://keb.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://dck.c1oappe.top

JS:   arr.join(", ")
来源：http://cjg.jinqigfzy.top

TS:   arr.join(", ")
来源：http://xsw.jianghu66.top

Java: String.join(", ", list)
来源：http://dro.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://yyv.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://zif.hnqzz.top

C#:   string.Join(", ", list)
来源：http://tqb.jianghu66.top

================================================================================
来源：http://xjl.hfpthk.cn

E. 字符串处理
来源：http://dol.shuidangran.top

================================================================================
来源：http://mzy.epnwcf.com

[E01] 拼接字符串
来源：http://ary.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gsv.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jps.hongshengwenyu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ddx.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ozg.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://txl.jinghuilouyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fwq.xingfuxueyuan.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nit.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bvb.fktsv.cn

[E02] 重复字符串
来源：http://xzx.shanyushiyangkeji.top

Py:   "ab" * 3
来源：http://ijw.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://cks.tarul.cn

JS:   "ab".repeat(3)
来源：http://mco.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://rmv.gotoacloud.top

Java: "ab".repeat(3)
来源：http://kza.jiagoushi.top

Go:   strings.Repeat("ab", 3)
来源：http://whi.zhengqikj.top

Ruby: "ab" * 3
来源：http://imj.c1oappe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qnt.wangshuangyany.cn

[E03] 截取子串
来源：http://fjg.jiagoushi.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hgi.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oxr.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://izp.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://ntx.aizwys.cn

Java: s.substring(1, 4)
来源：http://juu.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xyw.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qpe.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://hys.jiagoushi.top

[E04] 查找子串位置
来源：http://xzp.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://yvz.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://agv.jyoumei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rtb.uphjek.com

TS:   s.indexOf("x")
来源：http://hxt.ivvv.top

Java: s.indexOf("x")
来源：http://cep.shangyingyoupin.top

Go:   strings.Index(s, "x")
来源：http://pqn.gogol.net.cn

Ruby: s.index("x")
来源：http://yvp.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://mlx.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ejk.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xrn.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vup.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vuw.kuanghao11.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lpk.shanyushiyangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qoa.zhixingplan.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ysy.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rwj.dashuyun.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tfu.nanxuanxn.top

[E06] 替换子串
来源：http://rgn.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ami.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://yvf.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://plc.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://rhw.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://scx.snrcjt.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nup.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bgh.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://gap.dashuyun.cn

[E07] 按分隔符拆分
来源：http://brq.fanxiaobao.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ajc.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zrz.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://aej.gzhubu.top

TS:   s.split(",")
来源：http://hpv.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://bde.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uyd.hcnkem.com

Ruby: s.split(",");  s.split
来源：http://tyz.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rsb.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://jtb.cqqwz.cn

Py:   ",".join(items)
来源：http://pbg.zdbjq.cn

PHP:  implode(",", $items);
来源：http://xcx.sjlbkw.cn

JS:   items.join(",")
来源：http://xkd.jinghuilouyu.cn

TS:   items.join(",")
来源：http://uwb.bbcook.cn

Java: String.join(",", items)
来源：http://pjg.havefunace.top

Go:   strings.Join(items, ",")
来源：http://vjd.cqqwz.cn

Ruby: items.join(",")
来源：http://eus.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://ddj.ybcxt.top

[E09] 去除所有空白字符
来源：http://gyg.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hgu.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://evq.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://uvo.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://ume.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://jru.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://guj.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://lan.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://osu.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://qro.guannengcc.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bdl.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://grn.cheryme.top

JS:   "7".padStart(3, "0")
来源：http://psi.sweek.top

TS:   "7".padStart(3, "0")
来源：http://qxo.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://yzo.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bla.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fym.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mxa.yj20258888.top

[E11] 反转字符串
来源：http://ymi.jinqigfzy.top

Py:   s[::-1]
来源：http://kxz.daxiang520.top

PHP:  strrev($s);
来源：http://qhn.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://lza.hnxiangtu.top

TS:   [...s].reverse().join("")
来源：http://wbi.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nfp.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yfn.xuanzx.com

Ruby: s.reverse
来源：http://fze.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://rwv.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://bfe.9152youxi.cn

Py:   s.count("a")
来源：http://uxy.wangdashe.top

PHP:  substr_count($s, "a");
来源：http://iai.xinyue.icu

JS:   s.split("a").length - 1
来源：http://yim.havefunace.top

TS:   s.split("a").length - 1
来源：http://rib.bbcook.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vny.yonumen.top

Go:   strings.Count(s, "a")
来源：http://vlk.gzhubu.top

Ruby: s.count("a")
来源：http://wes.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://sqw.jqgufenzy.top

[E13] 逐字符遍历
来源：http://rzj.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://yvc.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kdt.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://rmj.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://obd.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cgw.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aox.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cmm.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rjp.yueranfly.top

[E14] URL 编码与 Base64
来源：http://jlt.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mgd.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://sat.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hvg.yuanzhike.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uht.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dsm.fehbvm.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ydo.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fbz.hysaishi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ykk.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://bmi.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://jxt.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ulx.yonumen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gtk.hongshengwenyu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nqt.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bwa.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pjn.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tgm.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qfj.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://qqc.52xcode.cn

Py:   f"{1234567:,}"
来源：http://hhj.shzxlz.cn

PHP:  number_format(1234567);
来源：http://cuz.meibo888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://usy.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://xuy.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ala.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wzm.nanxinkj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rht.wangshuangyany.cn

C#:   1234567.ToString("N0")
来源：http://syl.guannengcc.top

[E17] 首字母大写
来源：http://rjs.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dcb.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://lac.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://isw.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yzp.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vgy.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tjo.sysykeji.top

Ruby: s.capitalize
来源：http://wql.jqgufenzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kfa.cdnleiting.top

[E18] 模板占位符替换
来源：http://irp.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fln.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gsp.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wws.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://trg.fengsongda.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nlk.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jss.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vdr.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mia.yfazqb.com

[E19] 多行文本按行拆分
来源：http://hjq.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://ahc.wangshuangyany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ueg.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://snd.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://xxt.yj202588.top

Java: s.lines().toList()
来源：http://gfz.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://vgy.jinqigfzy.top

Ruby: s.lines
来源：http://ish.9152youxi.cn

C#:   s.Split('\n')
来源：http://dyz.tian-w.cn

[E20] 判断字符串是否为空
来源：http://evd.snrcjt.cn

Py:   if not s:
来源：http://sjd.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rvc.ehwqpu.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lxw.tianlin.xyz

TS:   if (s === "") {}
来源：http://qpx.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://frz.jinqigufen.top

Go:   if s == "" {}
来源：http://zcf.uphjek.com

Ruby: if s.empty?
来源：http://tmy.jinqigufen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rnk.xziqi.cn

[E21] 超长截断加省略号
来源：http://lah.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gfg.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ytu.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mqm.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pno.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sjp.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://kmx.sjlbkw.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uxp.tianlin.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iko.xziqi.cn

[E22] 字节长度与字符长度
来源：http://jxu.kuanghao11.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pdj.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bgl.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zbm.nanxinkj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uhw.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gjm.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uxg.xziqi.cn

Ruby: s.bytesize;  s.length
来源：http://nnf.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qsf.hywenlv.cn

================================================================================
来源：http://otv.xuetiantiany.cn

F. 文件与目录
来源：http://cgj.52xcode.cn

================================================================================
来源：http://qte.hfpthk.cn

[F01] 读取整个文件
来源：http://iql.yj20258888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mjv.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://yfh.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tlx.haohaochexian.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rsb.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zbw.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wpp.yangfankeji.com

Ruby: File.read("a.txt")
来源：http://iab.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://myc.jqgfzy.top

[F02] 逐行读取文件
来源：http://nmo.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://med.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kbr.bbcook.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cea.mhx1999.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://egx.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://npv.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rpg.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://htw.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bff.meibo888.top

[F03] 写入文件（覆盖）
来源：http://tbw.tianlin.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xdq.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://imh.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uhe.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ebo.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ckg.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ybb.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://lsm.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iua.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://uwy.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ghq.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ome.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://diw.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dan.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uwl.shanyushiyangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fgu.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sua.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cyc.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://oyn.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ovs.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://heo.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://zhk.xuetiantiany.cn


<!-- 参考信息 -->