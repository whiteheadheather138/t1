代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zjr.sysykeji.top

PHP:  array_merge(...$nested);
来源：http://kfa.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nud.yuanzhike.top

TS:   nested.flat();
来源：http://jky.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fpb.kuanghao11.cn

Go:   // 手写双层循环
来源：http://xpw.tarul.cn

Ruby: nested.flatten
来源：http://fbc.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pah.yuanzhike.top

[D19] 按字段分组
来源：http://woh.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qby.xingfuxueyuan.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://efm.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yon.chenjidiqi.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://mpy.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zbo.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://nhb.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vzz.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xfq.snrcjt.cn

[D20] 统计每个元素出现次数
来源：http://nsh.zhongyouzk.top

Py:   Counter(arr)
来源：http://lrj.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://cto.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sst.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://muq.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kvq.bjfxy.top

Go:   // 手写 map[T]int
来源：http://bdo.0kj1m.cn

Ruby: arr.tally
来源：http://lnk.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wvd.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://lfn.havefunace.top

Py:   x in arr
来源：http://hwh.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://hnb.jinqigfzy.top

JS:   arr.includes(x)
来源：http://prj.c1oappe.top

TS:   arr.includes(x)
来源：http://huk.gogol.net.cn

Java: list.contains(x)
来源：http://acj.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://jjk.sweek.top

Ruby: arr.include?(x)
来源：http://jvq.zdbjq.cn

C#:   list.Contains(x)
来源：http://bcf.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://fqn.mhx1999.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hgp.jinqigfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wkt.zhaomingkeji.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cpy.zhiwuduotai.top

TS:   [...arr];
来源：http://btv.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://wqf.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wto.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://jaq.zhixingplan.top

C#:   new List<int>(list);
来源：http://uyo.hesvh.cn

[D23] reduce 累积计算
来源：http://qhh.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lfe.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tgs.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gtm.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kvm.9152youxi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xuf.chenjidiqi.icu

Go:   // 手写循环
来源：http://vjr.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fmy.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nzm.tianlin.xyz

[D24] 字典 / Map 基本操作
来源：http://crx.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bvd.wangdashe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ynu.xuetiantiany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jvt.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ylf.yonumen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qgl.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kfp.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fsv.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qoi.ctjpmb.com

[D25] Set 集合去重与交并差
来源：http://ipo.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rli.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aec.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xsj.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lvu.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://skd.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mad.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cex.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ahy.yfazqb.com

[D26] 数组转字符串
来源：http://vxb.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://zwz.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://nse.yj20258888.top

JS:   arr.join(", ")
来源：http://qzv.hcnkem.com

TS:   arr.join(", ")
来源：http://lir.hywenlv.cn

Java: String.join(", ", list)
来源：http://avm.nanxinkj.top

Go:   strings.Join(strs, ", ")
来源：http://clm.yuanzhike.top

Ruby: arr.join(", ")
来源：http://hyb.bbcook.cn

C#:   string.Join(", ", list)
来源：http://piy.yvedp.cn

================================================================================
来源：http://kqm.9152youxi.cn

E. 字符串处理
来源：http://sww.cqqwz.cn

================================================================================
来源：http://wyi.ydjk.org.cn

[E01] 拼接字符串
来源：http://wzf.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aiu.snrcjt.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vnr.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mge.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wdo.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fyn.zycfv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lag.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zhu.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vkm.jianghu66.top

[E02] 重复字符串
来源：http://lmx.pycfn.com

Py:   "ab" * 3
来源：http://lqd.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://bzx.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://rtf.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://fho.sufxvd.cn

Java: "ab".repeat(3)
来源：http://shl.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://jrr.hywenlv.cn

Ruby: "ab" * 3
来源：http://eyc.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kvx.jqgfzy.top

[E03] 截取子串
来源：http://uat.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://txd.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qkc.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kzs.fengsongda.top

TS:   s.slice(1, 4)
来源：http://hhj.sysykeji.top

Java: s.substring(1, 4)
来源：http://ykq.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wra.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://cap.jianghu66.top

C#:   s.Substring(1, 3)
来源：http://bpb.yongpay.top

[E04] 查找子串位置
来源：http://boj.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://gvp.epnwcf.com

PHP:  strpos($s, "x");
来源：http://kfu.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qae.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://kjv.haohaochexian.top

Java: s.indexOf("x")
来源：http://bbe.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://agn.jianghu66.top

Ruby: s.index("x")
来源：http://izb.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://mis.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ijl.feifeiyinyue.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rrd.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kpa.xingfuxueyuan.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sko.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zkb.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://skh.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://khs.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qqz.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xwi.xinyue.icu

[E06] 替换子串
来源：http://opj.wangdashe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xba.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://lne.yfazqb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xnt.yongpay.top

TS:   s.replaceAll("a", "b")
来源：http://xuu.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vel.yuxming.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ryl.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://imj.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://vss.yfazqb.com

[E07] 按分隔符拆分
来源：http://nkw.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aoo.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zit.jinghuilouyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qua.bbcook.cn

TS:   s.split(",")
来源：http://moe.gogol.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pmp.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ykv.ywan-chungtsiang.top

Ruby: s.split(",");  s.split
来源：http://hyi.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://foz.sweek.top

[E08] 数组按分隔符合并
来源：http://wxg.pengpengdd.cyou

Py:   ",".join(items)
来源：http://dfc.ivvv.top

PHP:  implode(",", $items);
来源：http://pgg.birdmap.top

JS:   items.join(",")
来源：http://bov.cheryme.top

TS:   items.join(",")
来源：http://udz.cdnleiting.top

Java: String.join(",", items)
来源：http://ggt.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://mjc.xuetiantiany.cn

Ruby: items.join(",")
来源：http://yep.xziqi.cn

C#:   string.Join(",", items)
来源：http://tmz.aibaodan.cn

[E09] 去除所有空白字符
来源：http://yfe.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wfr.mhx1999.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bhk.tianlin.xyz

JS:   s.replace(/\s+/g, "")
来源：http://psy.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://vgc.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://mqr.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rss.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://hbo.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ojh.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://nmm.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xva.chenlongwang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rnk.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://yev.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://crg.shanyushiyangkeji.top

Java: String.format("%03d", 7)
来源：http://xrh.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pen.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dyv.sweek.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://psb.ppjwa.cn

[E11] 反转字符串
来源：http://evz.andypj.xyz

Py:   s[::-1]
来源：http://ttd.hfpthk.cn

PHP:  strrev($s);
来源：http://jbz.cashguo.top

JS:   [...s].reverse().join("")
来源：http://okv.fehbvm.com

TS:   [...s].reverse().join("")
来源：http://jcl.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aug.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://aok.shzxlz.cn

Ruby: s.reverse
来源：http://bvf.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://hxr.zycfv.cn

[E12] 统计某字符出现次数
来源：http://yvn.sjlbkw.cn

Py:   s.count("a")
来源：http://iap.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://dbf.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://qmb.c1oappe.top

TS:   s.split("a").length - 1
来源：http://ags.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qck.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://sor.fehbvm.com

Ruby: s.count("a")
来源：http://cwg.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://aki.hywenlv.cn

[E13] 逐字符遍历
来源：http://tbf.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://rcz.zhixingplan.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://etf.pycfn.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://xvi.fktsv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bpf.yuanzhike.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://anx.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pkg.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zve.yj20258888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pzi.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://uir.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cqe.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xyz.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://usa.zhongyouzk.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sak.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zsg.zycfv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://htn.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qqj.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ugk.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://eqf.andypj.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://zhz.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tvb.uphjek.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wnr.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nly.bbcook.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aln.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ubf.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tww.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qjl.redwolf501.top

[E16] 数字千分位
来源：http://xnv.yj20258888.top

Py:   f"{1234567:,}"
来源：http://lzo.bjfxy.top

PHP:  number_format(1234567);
来源：http://ehu.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://unp.xylfe.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oms.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kil.hysaishi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bbs.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://otz.pycfn.com

C#:   1234567.ToString("N0")
来源：http://ece.yonumen.top

[E17] 首字母大写
来源：http://wpl.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xzu.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ads.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cbq.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xkc.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hkm.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cis.kuanghao11.cn

Ruby: s.capitalize
来源：http://mom.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dqx.shuidangran.top

[E18] 模板占位符替换
来源：http://zka.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gok.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hbf.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://aji.sufxvd.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zya.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xdj.vehdjk.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wfk.dashuyun.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fbp.ydjk.org.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bst.c1oappe.top

[E19] 多行文本按行拆分
来源：http://wqi.yuanzhike.top

Py:   s.splitlines()
来源：http://trv.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://atj.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://thu.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://wit.zhengqikj.top

Java: s.lines().toList()
来源：http://bcu.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://xwe.shanyushiyangkeji.top

Ruby: s.lines
来源：http://nmo.jinqigufen.top

C#:   s.Split('\n')
来源：http://rtw.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://vld.hcnkem.com

Py:   if not s:
来源：http://zjf.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ogr.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lyx.jlsjyb.cn

TS:   if (s === "") {}
来源：http://kno.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://dcz.feifeiyinyue.top

Go:   if s == "" {}
来源：http://xdk.gogol.net.cn

Ruby: if s.empty?
来源：http://fdd.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sdw.fktsv.cn

[E21] 超长截断加省略号
来源：http://evf.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eup.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gln.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qpw.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vbs.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jhx.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://wyk.ydjk.org.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iot.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://efg.andypj.xyz

[E22] 字节长度与字符长度
来源：http://xdg.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nze.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zox.cqqwz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vbi.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bvt.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vcd.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://isf.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://ljh.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ntq.pengpengdd.cyou

================================================================================
来源：http://dwa.zhaomingkeji.xyz

F. 文件与目录
来源：http://jte.yueranfly.top

================================================================================
来源：http://flt.c1oappe.top

[F01] 读取整个文件
来源：http://ivm.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cqz.hongshengwenyu.top

PHP:  file_get_contents("a.txt");
来源：http://qqf.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tvu.nanxuanxn.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jbg.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://uhr.bbcook.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pfy.xylfe.cn

Ruby: File.read("a.txt")
来源：http://pek.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://mku.hfpthk.cn

[F02] 逐行读取文件
来源：http://vbt.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yow.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jeq.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xla.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tzt.gogol.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sbl.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://png.daria6918.cn


<!-- 参考信息 -->