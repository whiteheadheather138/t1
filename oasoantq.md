代发 wailian999

[D19] 按字段分组
来源：http://eqz.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://seq.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aoi.tianlin.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qhf.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yhw.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yxq.dianchejie.cn

Go:   // 手写 map[string][]T
来源：http://wwp.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://wvx.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bxv.cheryme.top

[D20] 统计每个元素出现次数
来源：http://ewe.xylfe.cn

Py:   Counter(arr)
来源：http://jkf.sxryk.cn

PHP:  array_count_values($arr);
来源：http://tms.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ryp.bbcook.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yvn.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qxk.yongpay.top

Go:   // 手写 map[T]int
来源：http://yax.yangfankeji.com

Ruby: arr.tally
来源：http://aqp.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hxy.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://ozw.mhx1999.top

Py:   x in arr
来源：http://ghv.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://zsi.yuxming.cn

JS:   arr.includes(x)
来源：http://jin.yj20258888.top

TS:   arr.includes(x)
来源：http://fja.yfazqb.com

Java: list.contains(x)
来源：http://tmd.jqgufenzy.top

Go:   slices.Contains(arr, x)
来源：http://lch.jianghu66.top

Ruby: arr.include?(x)
来源：http://lww.yuanzhike.top

C#:   list.Contains(x)
来源：http://ryw.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://jal.chenlongwang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tzh.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://agl.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cph.jinghuilouyu.cn

TS:   [...arr];
来源：http://gxp.haohaochexian.top

Java: new ArrayList<>(list);
来源：http://mgh.jianghu66.top

Go:   copied := append([]int(nil), arr...)
来源：http://wlh.smart0.xyz

Ruby: arr.dup;  arr.clone
来源：http://hgf.pengpengdd.cyou

C#:   new List<int>(list);
来源：http://clb.chenlongwang.top

[D23] reduce 累积计算
来源：http://wiz.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ulx.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wms.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iij.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wku.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://twy.fehbvm.com

Go:   // 手写循环
来源：http://tae.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nif.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qta.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://bit.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xdq.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gep.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tao.meibo888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zzp.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aah.xingfuxueyuan.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uzl.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rmn.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qwd.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://tit.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rzz.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pkh.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yes.hammf.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kdw.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zjt.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eyv.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hrk.haohaochexian.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mmr.yangfankeji.com

[D26] 数组转字符串
来源：http://wwb.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://lft.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://cnx.xziqi.cn

JS:   arr.join(", ")
来源：http://mfe.xinyue.icu

TS:   arr.join(", ")
来源：http://oia.vehdjk.com

Java: String.join(", ", list)
来源：http://pgf.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://kch.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://xxu.zycfv.cn

C#:   string.Join(", ", list)
来源：http://qcb.smart0.xyz

================================================================================
来源：http://fcz.gogol.net.cn

E. 字符串处理
来源：http://ptb.yfazqb.com

================================================================================
来源：http://qvh.316326.xyz

[E01] 拼接字符串
来源：http://ric.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xmf.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zsf.dashuyun.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ggn.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zqj.wangdashe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lem.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qtf.guannengcc.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qzk.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://amv.uphjek.com

[E02] 重复字符串
来源：http://kbf.yj202588.top

Py:   "ab" * 3
来源：http://aju.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://ljm.snrcjt.cn

JS:   "ab".repeat(3)
来源：http://loc.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://dfk.ybcxt.top

Java: "ab".repeat(3)
来源：http://jgf.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://nea.shuidangran.top

Ruby: "ab" * 3
来源：http://kvm.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://boq.9152youxi.cn

[E03] 截取子串
来源：http://ijj.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://esl.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ska.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://edx.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://zlk.fengsongda.top

Java: s.substring(1, 4)
来源：http://bwo.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://awt.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://fkq.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://tgb.nwbrower.top

[E04] 查找子串位置
来源：http://kul.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://rly.epnwcf.com

PHP:  strpos($s, "x");
来源：http://aku.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rln.hammf.cn

TS:   s.indexOf("x")
来源：http://fco.sysykeji.top

Java: s.indexOf("x")
来源：http://mzw.daria6918.cn

Go:   strings.Index(s, "x")
来源：http://ynl.shuidangran.top

Ruby: s.index("x")
来源：http://ejb.yj202588.top

C#:   s.IndexOf("x")
来源：http://ftx.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://uwm.yuanzhike.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jov.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wzd.zdqjudy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cam.xinyue.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://uxv.iojbl.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xuf.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qta.jyoumei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://phn.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vkr.xingfuxueyuan.xyz

[E06] 替换子串
来源：http://ijr.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tro.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://tmk.tarul.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dhd.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://tev.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fza.cucudq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://are.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gst.daxiang520.top

C#:   s.Replace("a", "b")
来源：http://zvv.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://wht.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rfe.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sse.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qqt.ybcxt.top

TS:   s.split(",")
来源：http://elk.gogol.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zbn.quarkkingdee.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bfh.guannengcc.top

Ruby: s.split(",");  s.split
来源：http://omk.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://efx.hnqzz.top

[E08] 数组按分隔符合并
来源：http://wco.c1oappe.top

Py:   ",".join(items)
来源：http://fpo.hywenlv.cn

PHP:  implode(",", $items);
来源：http://fpr.cdnleiting.top

JS:   items.join(",")
来源：http://bpy.yanxiufei.cn

TS:   items.join(",")
来源：http://qdo.zdqjudy.top

Java: String.join(",", items)
来源：http://vmh.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://vuy.guannengcc.top

Ruby: items.join(",")
来源：http://frp.tianlin.xyz

C#:   string.Join(",", items)
来源：http://szl.jlsjyb.cn

[E09] 去除所有空白字符
来源：http://prq.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tir.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ygt.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://tlj.feifeiyinyue.top

TS:   s.replace(/\s+/g, "")
来源：http://scu.snrcjt.cn

Java: s.replaceAll("\\s+", "")
来源：http://ihh.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wcx.bjfxy.top

Ruby: s.gsub(/\s+/, "")
来源：http://urq.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://igu.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://rpo.cdnleiting.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rgn.shanyushiyangtech.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://grf.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://vpi.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://vwp.redwolf501.top

Java: String.format("%03d", 7)
来源：http://dhv.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ruy.cashguo.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://unr.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wfx.hywenlv.cn

[E11] 反转字符串
来源：http://zbg.ydjk.org.cn

Py:   s[::-1]
来源：http://dzu.fengsongda.top

PHP:  strrev($s);
来源：http://wcz.yonumen.top

JS:   [...s].reverse().join("")
来源：http://wtg.meibo888.top

TS:   [...s].reverse().join("")
来源：http://bwx.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zjv.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xpk.sysykeji.top

Ruby: s.reverse
来源：http://ucs.ehwqpu.com

C#:   new string(s.Reverse().ToArray())
来源：http://klm.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://yog.yj202588.top

Py:   s.count("a")
来源：http://rcl.hongshengwenyu.top

PHP:  substr_count($s, "a");
来源：http://uwy.zhengqikj.top

JS:   s.split("a").length - 1
来源：http://vth.andypj.xyz

TS:   s.split("a").length - 1
来源：http://udv.smart0.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://red.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://iof.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://gib.hammf.cn

C#:   s.Count(c => c == 'a')
来源：http://qcn.guowangkeji.top

[E13] 逐字符遍历
来源：http://hal.aizwys.cn

Py:   for ch in s: print(ch)
来源：http://bxk.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://snb.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rne.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ded.uphjek.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ryx.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xxn.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://rnp.wangshuangyany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ohj.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://lye.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jqq.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://oek.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rer.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rfm.kuanghao11.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rfa.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://idc.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sze.feifeiyinyue.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hsh.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://gvt.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://rmp.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://akm.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://abh.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hkt.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ose.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bsn.zdbjq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yzu.feifeiyinyue.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ftu.yvedp.cn

[E16] 数字千分位
来源：http://dib.aizwys.cn

Py:   f"{1234567:,}"
来源：http://bhb.redwolf501.top

PHP:  number_format(1234567);
来源：http://spr.fzhhl.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lcy.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://knr.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yoy.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jee.yueranfly.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uiu.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://ofj.ehwqpu.com

[E17] 首字母大写
来源：http://enc.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ihg.shanyushiyangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://urf.jinqigufen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ndx.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ngp.hnxiangtu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rvj.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://trx.mhx1999.top

Ruby: s.capitalize
来源：http://epw.jqgufenzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qae.xziqi.cn

[E18] 模板占位符替换
来源：http://ruk.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cls.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cgy.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://waw.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oxs.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ivs.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zgq.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uzs.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lzt.feifeiyinyue.top

[E19] 多行文本按行拆分
来源：http://emj.0kj1m.cn

Py:   s.splitlines()
来源：http://xnl.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kjr.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://vgg.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://mtk.svipenyu.cn

Java: s.lines().toList()
来源：http://ejf.jinyuanbaomall.cn

Go:   strings.Split(s, "\n")
来源：http://vgl.wangdashe.top

Ruby: s.lines
来源：http://nfr.redwolf501.top

C#:   s.Split('\n')
来源：http://zcl.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://tws.hesvh.cn

Py:   if not s:
来源：http://rax.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nvk.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ubb.tianlin.xyz

TS:   if (s === "") {}
来源：http://vqq.svipenyu.cn

Java: if (s.isEmpty()) {}
来源：http://lyp.zhijiandao.cn

Go:   if s == "" {}
来源：http://jdm.hnxiangtu.top

Ruby: if s.empty?
来源：http://vmz.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dfj.xinyue.icu

[E21] 超长截断加省略号
来源：http://zza.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jmc.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://izr.nanxinkj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gaf.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kzy.ivvv.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://idb.vqdsnc.cn

Go:   // 按 rune 判断长度后截断
来源：http://glh.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://adr.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qgq.52xcode.cn

[E22] 字节长度与字符长度
来源：http://zew.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pzz.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yso.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yrv.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jgk.ppjwa.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dbh.aibaodan.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://unw.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://paf.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fju.tianlin.xyz

================================================================================
来源：http://fmz.zhaomingkeji.xyz

F. 文件与目录
来源：http://kjw.gaohongyu789.top

================================================================================
来源：http://hyn.hcnkem.com

[F01] 读取整个文件
来源：http://wuf.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://foa.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://bgy.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uxp.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uqh.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tks.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ybu.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://rqh.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://awi.zhengqikj.top

[F02] 逐行读取文件
来源：http://wyw.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gts.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hle.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eij.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eoq.fanxiaobao.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wjp.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zfd.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uep.hfpthk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oiv.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://byz.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xmg.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://app.zdqjudy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kkz.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vcl.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yoy.shuidangran.top


<!-- 参考信息 -->