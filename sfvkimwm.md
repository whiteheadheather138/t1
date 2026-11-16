代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yoz.zdbjq.cn

Go:   // 手写双层循环
来源：http://apy.cqqwz.cn

Ruby: nested.flatten
来源：http://mfl.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://jft.gotoacloud.top

[D19] 按字段分组
来源：http://nli.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hof.cqqwz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gnk.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vzg.yuanzhike.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ggq.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ugj.xylfe.cn

Go:   // 手写 map[string][]T
来源：http://hje.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://alh.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jxt.sufxvd.cn

[D20] 统计每个元素出现次数
来源：http://bnk.guannengcc.top

Py:   Counter(arr)
来源：http://sri.yueranfly.top

PHP:  array_count_values($arr);
来源：http://ywt.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rpm.svipenyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qit.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mdn.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://wxe.shangyingyoupin.top

Ruby: arr.tally
来源：http://uar.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rlv.cucudq.cn

[D21] 判断是否包含某元素
来源：http://zsu.havefunace.top

Py:   x in arr
来源：http://rrq.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://rrp.fanxiaobao.xyz

JS:   arr.includes(x)
来源：http://ecw.bbcook.cn

TS:   arr.includes(x)
来源：http://qvo.guowangkeji.top

Java: list.contains(x)
来源：http://ueb.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://wyg.nwbrower.top

Ruby: arr.include?(x)
来源：http://drw.tianlin.xyz

C#:   list.Contains(x)
来源：http://eft.jiagoushi.top

[D22] 复制数组（避免共享引用）
来源：http://kic.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jvt.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tac.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://glc.nanxuanxn.top

TS:   [...arr];
来源：http://rbp.uphjek.com

Java: new ArrayList<>(list);
来源：http://pxv.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qec.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://vvu.havefunace.top

C#:   new List<int>(list);
来源：http://ehn.xinyue.icu

[D23] reduce 累积计算
来源：http://zgy.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vcx.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ttm.jqgufenzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xwz.shanyushiyangtech.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hti.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://awp.redwolf501.top

Go:   // 手写循环
来源：http://stc.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vnu.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ixu.sufxvd.cn

[D24] 字典 / Map 基本操作
来源：http://vig.hysaishi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tpm.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fuw.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lfk.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xyo.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rpr.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://okp.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eut.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dux.cucudq.cn

[D25] Set 集合去重与交并差
来源：http://brj.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fkk.dianchejie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lii.fanxiaobao.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pka.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zqe.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xgq.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nxx.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kbu.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kbc.birdmap.top

[D26] 数组转字符串
来源：http://hud.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://cvu.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://sio.hysaishi.cn

JS:   arr.join(", ")
来源：http://wzc.xingfuxueyuan.xyz

TS:   arr.join(", ")
来源：http://ccm.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://bgp.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://krx.andypj.xyz

Ruby: arr.join(", ")
来源：http://asq.bbcook.cn

C#:   string.Join(", ", list)
来源：http://qis.wangshuangyany.cn

================================================================================
来源：http://jku.epnwcf.com

E. 字符串处理
来源：http://jut.ctjpmb.com

================================================================================
来源：http://idh.ctjpmb.com

[E01] 拼接字符串
来源：http://gwe.uphjek.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qli.tarul.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pfi.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uxl.smart0.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xtl.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hvm.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://smv.guowangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xld.fzhhl.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fxg.dianchejie.cn

[E02] 重复字符串
来源：http://alv.guowangkeji.top

Py:   "ab" * 3
来源：http://ben.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://jrh.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://cfu.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://sys.hammf.cn

Java: "ab".repeat(3)
来源：http://quu.mhx1999.top

Go:   strings.Repeat("ab", 3)
来源：http://qhi.ppjwa.cn

Ruby: "ab" * 3
来源：http://bsn.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jyb.yuxming.cn

[E03] 截取子串
来源：http://jxk.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bwc.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nad.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cyk.tarul.cn

TS:   s.slice(1, 4)
来源：http://vso.daxiang520.top

Java: s.substring(1, 4)
来源：http://kvq.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uup.jinqigfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://wbt.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://acb.hfpthk.cn

[E04] 查找子串位置
来源：http://pts.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://tgr.tarul.cn

PHP:  strpos($s, "x");
来源：http://ztd.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://riq.vehdjk.com

TS:   s.indexOf("x")
来源：http://ctu.sweek.top

Java: s.indexOf("x")
来源：http://fps.yueranfly.top

Go:   strings.Index(s, "x")
来源：http://bqy.xinyue.icu

Ruby: s.index("x")
来源：http://xdn.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://opp.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://una.yuanzhike.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kdl.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ggg.chenzaomai.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dcj.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mow.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rws.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ivc.yvedp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uzp.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bpi.yj20258888.top

[E06] 替换子串
来源：http://hyw.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://okr.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://byy.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gmt.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://ipi.zhaomingkeji.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oke.kuanghao11.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://caz.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://swz.jyoumei.cn

C#:   s.Replace("a", "b")
来源：http://ivi.tian-w.cn

[E07] 按分隔符拆分
来源：http://gtt.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://thx.zhaomingkeji.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tob.zhengqikj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gke.kuanghao11.cn

TS:   s.split(",")
来源：http://bqv.cucudq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vty.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uik.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://erg.0kj1m.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://juw.gogol.net.cn

[E08] 数组按分隔符合并
来源：http://nlk.yvedp.cn

Py:   ",".join(items)
来源：http://pll.sweek.top

PHP:  implode(",", $items);
来源：http://ked.bjfxy.top

JS:   items.join(",")
来源：http://kss.kuanghao11.cn

TS:   items.join(",")
来源：http://otb.ydjk.org.cn

Java: String.join(",", items)
来源：http://azf.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://xwn.jlsjyb.cn

Ruby: items.join(",")
来源：http://fbx.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://miv.hywenlv.cn

[E09] 去除所有空白字符
来源：http://ixq.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qer.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cac.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://hgk.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://cre.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://smh.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ucr.quarkkingdee.top

Ruby: s.gsub(/\s+/, "")
来源：http://vup.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yaw.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://gno.cqqwz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://was.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://crf.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://byk.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://akj.nwbrower.top

Java: String.format("%03d", 7)
来源：http://ste.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tcb.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dzc.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qej.fehbvm.com

[E11] 反转字符串
来源：http://dww.yuxming.cn

Py:   s[::-1]
来源：http://mau.jqgufenzy.top

PHP:  strrev($s);
来源：http://gda.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://ixc.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://bgm.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ubm.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kpu.feifeiyinyue.top

Ruby: s.reverse
来源：http://zfw.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xuu.pycfn.com

[E12] 统计某字符出现次数
来源：http://twn.yfazqb.com

Py:   s.count("a")
来源：http://uld.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://uvq.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://vvk.tanke756.top

TS:   s.split("a").length - 1
来源：http://uar.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dnb.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://dmn.kuanghao11.cn

Ruby: s.count("a")
来源：http://hbk.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://efz.sjlbkw.cn

[E13] 逐字符遍历
来源：http://ryc.svipenyu.cn

Py:   for ch in s: print(ch)
来源：http://wsc.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lxt.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tco.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ocy.hcnkem.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ymy.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://piy.zdbjq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rnk.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tnk.wangdashe.top

[E14] URL 编码与 Base64
来源：http://joc.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xxg.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rid.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rle.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://duv.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kwz.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fzm.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://udw.sufxvd.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://snn.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://ncj.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://bzk.gogol.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cep.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wyb.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zfp.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ybb.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://inh.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://syf.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wny.0kj1m.cn

[E16] 数字千分位
来源：http://sir.fktsv.cn

Py:   f"{1234567:,}"
来源：http://rcs.fzhhl.top

PHP:  number_format(1234567);
来源：http://gpo.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://grs.hysaishi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nxg.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tbi.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ykp.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://udq.daxiang520.top

C#:   1234567.ToString("N0")
来源：http://dke.zdbjq.cn

[E17] 首字母大写
来源：http://brc.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ilc.daria6918.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cjb.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aku.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wpq.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wox.jianghu66.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lrj.xuetiantiany.cn

Ruby: s.capitalize
来源：http://mdq.haohaochexian.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ugq.chenlongwang.top

[E18] 模板占位符替换
来源：http://yst.shangyingyoupin.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://toz.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wnv.havefunace.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wkg.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://ixu.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://msr.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://frs.tian-w.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dxf.fehbvm.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nnd.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://osl.iojbl.cn

Py:   s.splitlines()
来源：http://xvh.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xam.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://xvl.xylfe.cn

TS:   s.split(/\r?\n/)
来源：http://pwr.yueranfly.top

Java: s.lines().toList()
来源：http://rhf.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://pws.snrcjt.cn

Ruby: s.lines
来源：http://oyl.jinqigufen.top

C#:   s.Split('\n')
来源：http://nde.cucudq.cn

[E20] 判断字符串是否为空
来源：http://vfp.zhixingplan.top

Py:   if not s:
来源：http://sjs.hammf.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rqi.jlsjyb.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kcw.shanyushiyangtech.top

TS:   if (s === "") {}
来源：http://ume.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://jyv.uphjek.com

Go:   if s == "" {}
来源：http://xsh.shzxlz.cn

Ruby: if s.empty?
来源：http://qhr.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hjc.gzhubu.top

[E21] 超长截断加省略号
来源：http://ikn.zhixingplan.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qqf.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qbc.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wky.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cxa.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fic.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://awk.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uvb.c1oappe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pzw.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://vxu.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dwb.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://trc.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vzk.haohaochexian.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uak.sweek.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vuz.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kki.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://pfz.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cdd.iojbl.cn

================================================================================
来源：http://gtp.yvedp.cn

F. 文件与目录
来源：http://xnf.pycfn.com

================================================================================
来源：http://uvl.tian-w.cn

[F01] 读取整个文件
来源：http://bft.yanxiufei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://czc.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://ofm.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://clb.yangfankeji.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zdp.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cgt.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xnu.gzhubu.top

Ruby: File.read("a.txt")
来源：http://tly.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://qtf.yj202588.top

[F02] 逐行读取文件
来源：http://lhq.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vft.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wmw.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://naz.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fbp.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iuy.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tmt.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jiw.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vuf.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://wwk.nanxuanxn.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xbc.cashguo.top


<!-- 参考信息 -->