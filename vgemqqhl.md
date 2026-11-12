代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://otn.svipenyu.cn

[D20] 统计每个元素出现次数
来源：http://pfk.c1oappe.top

Py:   Counter(arr)
来源：http://ibt.bbcook.cn

PHP:  array_count_values($arr);
来源：http://ffx.sysykeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bmd.cdnleiting.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://utv.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://loc.yvedp.cn

Go:   // 手写 map[T]int
来源：http://ejb.aizwys.cn

Ruby: arr.tally
来源：http://ipt.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qlc.guannengcc.top

[D21] 判断是否包含某元素
来源：http://evs.hcnkem.com

Py:   x in arr
来源：http://xfe.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://cbl.dashuyun.cn

JS:   arr.includes(x)
来源：http://lyz.ybcxt.top

TS:   arr.includes(x)
来源：http://tfe.aibaodan.cn

Java: list.contains(x)
来源：http://oxv.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://wzt.yj20258.top

Ruby: arr.include?(x)
来源：http://oaq.ivvv.top

C#:   list.Contains(x)
来源：http://ptx.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://ien.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rkd.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wxh.pycfn.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zlx.havefunace.top

TS:   [...arr];
来源：http://fji.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://kqb.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://kkn.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://cnm.birdmap.top

C#:   new List<int>(list);
来源：http://kpd.zhixingplan.top

[D23] reduce 累积计算
来源：http://ouk.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cye.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cwz.yvedp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bth.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kau.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://dsx.feifeiyinyue.top

Go:   // 手写循环
来源：http://szm.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jin.ppjwa.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dpo.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://ial.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fpl.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zfx.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zdu.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vue.bbcook.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tuv.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pwi.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fob.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wlt.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://yow.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://skw.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://khz.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cej.zhixingplan.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://loj.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://alo.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rdb.birdmap.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xbp.c1oappe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://teh.daxiang520.top

[D26] 数组转字符串
来源：http://hug.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://iqv.zhengqikj.top

PHP:  implode(", ", $arr);
来源：http://ksw.zhixingplan.top

JS:   arr.join(", ")
来源：http://yut.yanxiufei.cn

TS:   arr.join(", ")
来源：http://iiu.quarkkingdee.top

Java: String.join(", ", list)
来源：http://jmy.jinyuanbaomall.cn

Go:   strings.Join(strs, ", ")
来源：http://uch.svipenyu.cn

Ruby: arr.join(", ")
来源：http://xkk.xuanzx.com

C#:   string.Join(", ", list)
来源：http://weq.c1oappe.top

================================================================================
来源：http://isv.aizwys.cn

E. 字符串处理
来源：http://jrr.jinghuilouyu.cn

================================================================================
来源：http://alg.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://gvd.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cxu.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://col.fanxiaobao.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fas.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://evr.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vst.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tyn.wangshuangyany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://euz.tarul.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wlo.zhixingplan.top

[E02] 重复字符串
来源：http://fit.ehwqpu.com

Py:   "ab" * 3
来源：http://fre.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://liv.sweek.top

JS:   "ab".repeat(3)
来源：http://acu.guowangkeji.top

TS:   "ab".repeat(3)
来源：http://qvo.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://tyw.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://egr.bbcook.cn

Ruby: "ab" * 3
来源：http://vkv.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://acx.yj20258888.top

[E03] 截取子串
来源：http://ssz.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wru.vqdsnc.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pqo.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cmx.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://dlh.zycfv.cn

Java: s.substring(1, 4)
来源：http://tpt.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vby.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yvx.zdbjq.cn

C#:   s.Substring(1, 3)
来源：http://hdf.daria6918.cn

[E04] 查找子串位置
来源：http://lmg.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://rne.ydzc1.top

PHP:  strpos($s, "x");
来源：http://uhb.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fbe.xuanzx.com

TS:   s.indexOf("x")
来源：http://fup.zhoulong.xyz

Java: s.indexOf("x")
来源：http://rem.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://lwr.hnxiangtu.top

Ruby: s.index("x")
来源：http://msv.zycfv.cn

C#:   s.IndexOf("x")
来源：http://bbf.nwbrower.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bho.zhongyouzk.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://igq.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://msw.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://psv.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kqf.meibo888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://boj.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dxb.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://puh.dianchejie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fys.zhijiandao.cn

[E06] 替换子串
来源：http://stg.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uqk.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://wsj.zhongyouzk.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fez.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://xoj.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xkb.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vdi.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://czb.sjlbkw.cn

C#:   s.Replace("a", "b")
来源：http://jwk.redwolf501.top

[E07] 按分隔符拆分
来源：http://ssi.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nct.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ayy.ydjk.org.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mxb.guannengcc.top

TS:   s.split(",")
来源：http://zri.yangfankeji.com

Java: s.split(",");  s.split("\\s+")
来源：http://qll.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://opz.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://wdt.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rli.cdnleiting.top

[E08] 数组按分隔符合并
来源：http://gif.tarul.cn

Py:   ",".join(items)
来源：http://ikm.9152youxi.cn

PHP:  implode(",", $items);
来源：http://der.jqgfzy.top

JS:   items.join(",")
来源：http://izc.hongshengwenyu.top

TS:   items.join(",")
来源：http://gxh.kuanghao11.cn

Java: String.join(",", items)
来源：http://xzb.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://nvj.yvedp.cn

Ruby: items.join(",")
来源：http://gqp.birdmap.top

C#:   string.Join(",", items)
来源：http://otb.yangfankeji.com

[E09] 去除所有空白字符
来源：http://qnh.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wey.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xug.hesvh.cn

JS:   s.replace(/\s+/g, "")
来源：http://igt.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://vdo.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://xhz.yanxiufei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://keq.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://sse.iojbl.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://slm.pengpengdd.cyou

[E10] 左侧补零 / 定长填充
来源：http://lph.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cyh.yongpay.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://syl.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://nsi.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://jlm.52xcode.cn

Java: String.format("%03d", 7)
来源：http://rbf.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fhz.chenzaomai.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cur.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kvc.nanxinkj.top

[E11] 反转字符串
来源：http://ffx.zhijiandao.cn

Py:   s[::-1]
来源：http://xrh.fehbvm.com

PHP:  strrev($s);
来源：http://dan.xylfe.cn

JS:   [...s].reverse().join("")
来源：http://cde.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://zwy.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sll.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bfh.52xcode.cn

Ruby: s.reverse
来源：http://lel.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vse.cdnleiting.top

[E12] 统计某字符出现次数
来源：http://pjy.jqgfzy.top

Py:   s.count("a")
来源：http://bxg.chenjidiqi.icu

PHP:  substr_count($s, "a");
来源：http://rmq.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://beg.guannengcc.top

TS:   s.split("a").length - 1
来源：http://yhe.nanxinkj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bhj.zycfv.cn

Go:   strings.Count(s, "a")
来源：http://qva.feifeiyinyue.top

Ruby: s.count("a")
来源：http://ost.tarul.cn

C#:   s.Count(c => c == 'a')
来源：http://wyp.gotoacloud.top

[E13] 逐字符遍历
来源：http://fky.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://hvm.cheryme.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cgk.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kkc.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tfy.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iif.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oqh.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bvl.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dix.birdmap.top

[E14] URL 编码与 Base64
来源：http://qud.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qcz.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iyd.xingfuxueyuan.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rfy.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://buc.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tdv.chenzaomai.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://skp.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vbx.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qus.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://otl.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zio.iojbl.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sav.jinghuilouyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vri.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://has.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bju.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bzf.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uxj.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fpo.vqdsnc.cn

[E16] 数字千分位
来源：http://dev.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://ecb.haohaochexian.top

PHP:  number_format(1234567);
来源：http://ojn.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vbp.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mpf.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pod.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yre.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qml.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://eev.pengpengdd.cyou

[E17] 首字母大写
来源：http://wmx.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tby.hcnkem.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://uqz.pycfn.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wly.hnqzz.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blf.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://osq.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wzc.xinyue.icu

Ruby: s.capitalize
来源：http://hht.ydzc1.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yjo.dianchejie.cn

[E18] 模板占位符替换
来源：http://pgn.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ffe.0kj1m.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vfo.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bwb.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fxd.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kob.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xge.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mwv.fehbvm.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bfm.redwolf501.top

[E19] 多行文本按行拆分
来源：http://ncl.nanxinkj.top

Py:   s.splitlines()
来源：http://nsf.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gfg.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://mmq.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://kvk.vehdjk.com

Java: s.lines().toList()
来源：http://odc.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://qkf.sweek.top

Ruby: s.lines
来源：http://jxy.ivvv.top

C#:   s.Split('\n')
来源：http://fgm.316326.xyz

[E20] 判断字符串是否为空
来源：http://ffo.svipenyu.cn

Py:   if not s:
来源：http://hko.wangshuangyany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yln.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ibg.iojbl.cn

TS:   if (s === "") {}
来源：http://ovk.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://iri.c1oappe.top

Go:   if s == "" {}
来源：http://izm.smart0.xyz

Ruby: if s.empty?
来源：http://lof.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://upv.ydzc1.top

[E21] 超长截断加省略号
来源：http://hxx.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ged.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wnu.meibo888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kuk.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xfk.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fss.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://dtv.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ijq.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iql.tanke756.top

[E22] 字节长度与字符长度
来源：http://idz.smart0.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wti.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://piz.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uqs.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hmt.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kbd.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vxo.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://mpw.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://svt.yj20258888.top

================================================================================
来源：http://cii.shuidangran.top

F. 文件与目录
来源：http://kmg.andypj.xyz

================================================================================
来源：http://brz.zycfv.cn

[F01] 读取整个文件
来源：http://zgy.sweek.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pln.chenzaomai.com

PHP:  file_get_contents("a.txt");
来源：http://czt.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bgn.yuxming.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://coi.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://ejd.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yoi.52xcode.cn

Ruby: File.read("a.txt")
来源：http://pah.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://fcr.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://ece.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xoh.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oeo.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zuk.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tjn.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yhd.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eqe.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yxs.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jrf.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://jkc.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tjw.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rvj.andypj.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uga.snrcjt.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oss.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://igc.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yff.tarul.cn

Ruby: File.write("a.txt", "hi")
来源：http://kwr.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kzk.cheryme.top

[F04] 追加写入文件
来源：http://amw.ivvv.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://djg.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://evi.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kvr.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wmy.nwbrower.top


<!-- 参考信息 -->