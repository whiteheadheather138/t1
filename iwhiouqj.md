代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qab.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://med.0kj1m.cn

Py:   Counter(arr)
来源：http://irb.yangfankeji.com

PHP:  array_count_values($arr);
来源：http://ttf.kuanghao11.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nba.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mba.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://guh.cucudq.cn

Go:   // 手写 map[T]int
来源：http://rkm.tian-w.cn

Ruby: arr.tally
来源：http://gvs.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jkr.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://evb.tarul.cn

Py:   x in arr
来源：http://hyo.ybcxt.top

PHP:  in_array($x, $arr, true);
来源：http://jxf.zhixingplan.top

JS:   arr.includes(x)
来源：http://ltq.snrcjt.cn

TS:   arr.includes(x)
来源：http://vpc.bjfxy.top

Java: list.contains(x)
来源：http://mnu.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://ymr.shuidangran.top

Ruby: arr.include?(x)
来源：http://sji.sweek.top

C#:   list.Contains(x)
来源：http://rak.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://rcm.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://onv.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zhi.ydjk.org.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ecc.yj20258.top

TS:   [...arr];
来源：http://dsc.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://xim.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://orb.xuetiantiany.cn

Ruby: arr.dup;  arr.clone
来源：http://kxc.chenzaomai.com

C#:   new List<int>(list);
来源：http://fkx.yj202588.top

[D23] reduce 累积计算
来源：http://vkm.xinyue.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bol.jqgfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oqx.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xzz.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://azl.havefunace.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qpa.fanxiaobao.xyz

Go:   // 手写循环
来源：http://tfy.pengpengdd.cyou

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hht.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uic.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://wxn.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wfy.jinyuanbaomall.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iae.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bhy.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xan.wangdashe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fos.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jbd.xinyue.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jnv.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gkt.316326.xyz

[D25] Set 集合去重与交并差
来源：http://ems.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lhf.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tkg.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vyq.zhengqikj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ijx.cheryme.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hkn.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qop.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wwg.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://poc.nanxinkj.top

[D26] 数组转字符串
来源：http://wpk.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://nlk.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://eil.cucudq.cn

JS:   arr.join(", ")
来源：http://ivp.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://usj.ppjwa.cn

Java: String.join(", ", list)
来源：http://adk.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://cwi.zdbjq.cn

Ruby: arr.join(", ")
来源：http://bjy.tarul.cn

C#:   string.Join(", ", list)
来源：http://kzj.pengpengdd.cyou

================================================================================
来源：http://bph.ctjpmb.com

E. 字符串处理
来源：http://axy.zhongyouzk.top

================================================================================
来源：http://wbx.nwbrower.top

[E01] 拼接字符串
来源：http://cel.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gvp.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zsa.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rxg.vehdjk.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ole.xuanzx.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nac.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mka.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pcv.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fii.zycfv.cn

[E02] 重复字符串
来源：http://ksh.smart0.xyz

Py:   "ab" * 3
来源：http://laa.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://yob.ybcxt.top

JS:   "ab".repeat(3)
来源：http://ngy.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://mdh.yuanzhike.top

Java: "ab".repeat(3)
来源：http://qof.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://hza.yuanzhike.top

Ruby: "ab" * 3
来源：http://tne.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uvm.zhaomingkeji.xyz

[E03] 截取子串
来源：http://dmv.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tnp.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://unv.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ciq.sysykeji.top

TS:   s.slice(1, 4)
来源：http://hws.jianghu66.top

Java: s.substring(1, 4)
来源：http://rxv.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zck.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://kog.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://flb.daria6918.cn

[E04] 查找子串位置
来源：http://byv.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://tjd.bbcook.cn

PHP:  strpos($s, "x");
来源：http://xbm.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fgg.sufxvd.cn

TS:   s.indexOf("x")
来源：http://esw.havefunace.top

Java: s.indexOf("x")
来源：http://zat.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://ygu.ydzc1.top

Ruby: s.index("x")
来源：http://tdy.jqgufenzy.top

C#:   s.IndexOf("x")
来源：http://hxg.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xki.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://agk.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eas.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aba.zhijiandao.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://seo.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hhz.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vvq.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://flg.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ilm.wangshuangyany.cn

[E06] 替换子串
来源：http://uof.ydjk.org.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rkx.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://iel.aibaodan.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dvv.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://yua.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://njn.cucudq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://klz.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nxg.guannengcc.top

C#:   s.Replace("a", "b")
来源：http://usm.smart0.xyz

[E07] 按分隔符拆分
来源：http://cab.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://feg.yonumen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ogg.mhx1999.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qxu.mhx1999.top

TS:   s.split(",")
来源：http://bhw.ydjk.org.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ure.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pxs.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://qpo.ydjk.org.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xsd.tanke756.top

[E08] 数组按分隔符合并
来源：http://lck.yfazqb.com

Py:   ",".join(items)
来源：http://pdh.nwbrower.top

PHP:  implode(",", $items);
来源：http://ffs.9152youxi.cn

JS:   items.join(",")
来源：http://rsf.zhoulong.xyz

TS:   items.join(",")
来源：http://bhf.haohaochexian.top

Java: String.join(",", items)
来源：http://kaj.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://cpo.zhengqikj.top

Ruby: items.join(",")
来源：http://vem.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://sox.haohaochexian.top

[E09] 去除所有空白字符
来源：http://mgw.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nmt.andypj.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sfa.zhengqikj.top

JS:   s.replace(/\s+/g, "")
来源：http://gzk.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://aiu.ctjpmb.com

Java: s.replaceAll("\\s+", "")
来源：http://pts.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hgm.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wjg.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fmw.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://qpu.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wey.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dna.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://kap.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://smn.yj202588.top

Java: String.format("%03d", 7)
来源：http://gli.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tyz.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ync.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gff.gzhubu.top

[E11] 反转字符串
来源：http://fez.yj20258.top

Py:   s[::-1]
来源：http://qom.vqdsnc.cn

PHP:  strrev($s);
来源：http://syc.vehdjk.com

JS:   [...s].reverse().join("")
来源：http://gsd.gotoacloud.top

TS:   [...s].reverse().join("")
来源：http://lyp.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dic.9152youxi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ovi.yongpay.top

Ruby: s.reverse
来源：http://jfa.kuanghao11.cn

C#:   new string(s.Reverse().ToArray())
来源：http://all.tanke756.top

[E12] 统计某字符出现次数
来源：http://fxs.feifeiyinyue.top

Py:   s.count("a")
来源：http://ydq.jyoumei.cn

PHP:  substr_count($s, "a");
来源：http://ffz.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://kpy.sysykeji.top

TS:   s.split("a").length - 1
来源：http://jnh.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mqv.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://mfq.hongshengwenyu.top

Ruby: s.count("a")
来源：http://cwd.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://kpw.tianlin.xyz

[E13] 逐字符遍历
来源：http://dve.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://ezd.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vge.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tfw.jianghu66.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bjb.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zhz.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://biy.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vgj.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aah.yueranfly.top

[E14] URL 编码与 Base64
来源：http://dpe.jinyuanbaomall.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yez.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gxy.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nud.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gyp.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bef.c1oappe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yhd.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bnu.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lur.dianchejie.cn

[E15] HTML 转义 / 反转义
来源：http://voz.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bgq.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hpb.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zct.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xra.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pej.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zur.birdmap.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qdz.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://odw.nanxinkj.top

[E16] 数字千分位
来源：http://ubc.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://hix.yvedp.cn

PHP:  number_format(1234567);
来源：http://hvy.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pba.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zkr.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yji.guowangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cda.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qtn.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://adm.sjlbkw.cn

[E17] 首字母大写
来源：http://fha.xuanzx.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://npk.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uht.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xte.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vbg.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pxo.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xlf.sxryk.cn

Ruby: s.capitalize
来源：http://kmt.jiagoushi.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uwb.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://vgi.52xcode.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hyr.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gxf.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gnv.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hbc.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aoe.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://guf.zhijiandao.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nhy.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fpu.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://lqp.yueranfly.top

Py:   s.splitlines()
来源：http://nao.quarkkingdee.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cgn.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://nwt.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://iny.nanxuanxn.top

Java: s.lines().toList()
来源：http://wdo.epnwcf.com

Go:   strings.Split(s, "\n")
来源：http://bam.ydzc1.top

Ruby: s.lines
来源：http://tdl.hfpthk.cn

C#:   s.Split('\n')
来源：http://ibp.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://vjo.jianghu66.top

Py:   if not s:
来源：http://ojm.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://boi.gotoacloud.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dpe.hfpthk.cn

TS:   if (s === "") {}
来源：http://bqe.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://uix.hfpthk.cn

Go:   if s == "" {}
来源：http://ydc.cashguo.top

Ruby: if s.empty?
来源：http://dfp.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bir.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://txs.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bsc.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mnt.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nsy.daria6918.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qju.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xjd.ppjwa.cn

Go:   // 按 rune 判断长度后截断
来源：http://glf.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jfr.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zxv.xuanzx.com

[E22] 字节长度与字符长度
来源：http://lgp.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ysw.sysykeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bup.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qlm.hnqzz.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pll.jinghuilouyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://esx.mhx1999.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bzv.hywenlv.cn

Ruby: s.bytesize;  s.length
来源：http://vst.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nve.shzxlz.cn

================================================================================
来源：http://uqd.shanyushiyangkeji.top

F. 文件与目录
来源：http://elh.jinqigfzy.top

================================================================================
来源：http://aoa.mhx1999.top

[F01] 读取整个文件
来源：http://xrb.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hwi.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://qmo.cucudq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zfo.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dbf.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hay.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://flh.yj20258888.top

Ruby: File.read("a.txt")
来源：http://ckn.0kj1m.cn

C#:   File.ReadAllText("a.txt");
来源：http://bsz.fktsv.cn

[F02] 逐行读取文件
来源：http://fbj.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nkn.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zcz.iojbl.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://agy.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xwr.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://joz.cdnleiting.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kjl.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yuv.dianchejie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oyk.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://lyu.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ksi.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lki.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://swo.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yum.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://itt.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ufv.yangfankeji.com

Ruby: File.write("a.txt", "hi")
来源：http://ewd.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zmi.cheryme.top

[F04] 追加写入文件
来源：http://job.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://odw.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qnc.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ewi.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://evv.feifeiyinyue.top


<!-- 参考信息 -->