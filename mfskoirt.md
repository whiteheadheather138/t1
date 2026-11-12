代发 wailian999

[D19] 按字段分组
来源：http://jxu.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fvy.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xvl.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rvo.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mia.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kny.xylfe.cn

Go:   // 手写 map[string][]T
来源：http://rju.ydjk.org.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://apa.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rft.hysaishi.cn

[D20] 统计每个元素出现次数
来源：http://isp.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://pcl.yfazqb.com

PHP:  array_count_values($arr);
来源：http://oja.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ttf.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hbv.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wmn.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://tgj.xingfuxueyuan.xyz

Ruby: arr.tally
来源：http://acv.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ndk.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://kno.fzhhl.top

Py:   x in arr
来源：http://xrt.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://jkk.fengsongda.top

JS:   arr.includes(x)
来源：http://gtq.zycfv.cn

TS:   arr.includes(x)
来源：http://pfl.zhixingplan.top

Java: list.contains(x)
来源：http://naq.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://mpw.yj20258888.top

Ruby: arr.include?(x)
来源：http://kgc.hesvh.cn

C#:   list.Contains(x)
来源：http://fhi.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://lls.kuanghao11.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fwr.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yjt.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sko.daxiang520.top

TS:   [...arr];
来源：http://bxq.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://oyf.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pxe.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://xmo.hnqzz.top

C#:   new List<int>(list);
来源：http://jsg.xylfe.cn

[D23] reduce 累积计算
来源：http://auz.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://evg.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pav.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aco.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zco.shuidangran.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pfe.zdbjq.cn

Go:   // 手写循环
来源：http://jtn.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lqx.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vug.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://add.ppjwa.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ytp.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ilb.xingfuxueyuan.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://svz.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ttc.xuanzx.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iyc.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ael.cdnleiting.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fql.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yld.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://ffr.feifeiyinyue.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://foi.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rvg.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cyu.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oyt.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xvx.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lsy.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xqg.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yct.ehwqpu.com

[D26] 数组转字符串
来源：http://qhl.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://xsd.ydjk.org.cn

PHP:  implode(", ", $arr);
来源：http://grc.jqgfzy.top

JS:   arr.join(", ")
来源：http://tjf.nwbrower.top

TS:   arr.join(", ")
来源：http://joc.aizwys.cn

Java: String.join(", ", list)
来源：http://tyv.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://ryo.zycfv.cn

Ruby: arr.join(", ")
来源：http://lnr.andypj.xyz

C#:   string.Join(", ", list)
来源：http://rxy.shanyushiyangkeji.top

================================================================================
来源：http://jpc.tanke756.top

E. 字符串处理
来源：http://vuc.xuanzx.com

================================================================================
来源：http://nkq.52xcode.cn

[E01] 拼接字符串
来源：http://xus.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ikv.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ash.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rpf.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kqz.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vvg.daxiang520.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://omk.yangfankeji.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mqz.daria6918.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://umq.wangdashe.top

[E02] 重复字符串
来源：http://mhe.uphjek.com

Py:   "ab" * 3
来源：http://kla.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://llc.zhengqikj.top

JS:   "ab".repeat(3)
来源：http://ygm.yvedp.cn

TS:   "ab".repeat(3)
来源：http://jui.316326.xyz

Java: "ab".repeat(3)
来源：http://tqt.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://nda.ydzc1.top

Ruby: "ab" * 3
来源：http://taw.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xvx.ppjwa.cn

[E03] 截取子串
来源：http://skc.zdbjq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gah.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fpa.zhengqikj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lmv.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://kbz.yangfankeji.com

Java: s.substring(1, 4)
来源：http://lsp.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qmj.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://jsy.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://bvw.jinqigfzy.top

[E04] 查找子串位置
来源：http://wac.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://khp.epnwcf.com

PHP:  strpos($s, "x");
来源：http://wlp.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iib.fktsv.cn

TS:   s.indexOf("x")
来源：http://uzf.ydjk.org.cn

Java: s.indexOf("x")
来源：http://ywe.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://rlr.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://gqq.hnxiangtu.top

C#:   s.IndexOf("x")
来源：http://etg.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://aqm.fanxiaobao.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qtd.yj20258888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hqr.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oxh.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eih.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kfu.quarkkingdee.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bgq.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hia.feifeiyinyue.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gya.fktsv.cn

[E06] 替换子串
来源：http://vap.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eku.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://zxx.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dqm.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://loe.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wbv.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xef.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://txu.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://aeu.bbcook.cn

[E07] 按分隔符拆分
来源：http://beg.shangyingyoupin.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://knj.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lik.yangfankeji.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://fiw.jyoumei.cn

TS:   s.split(",")
来源：http://cnw.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ock.hammf.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cfn.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://dqx.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yvi.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://rlv.jlsjyb.cn

Py:   ",".join(items)
来源：http://qtk.havefunace.top

PHP:  implode(",", $items);
来源：http://xvw.ydzc1.top

JS:   items.join(",")
来源：http://bbl.nanxuanxn.top

TS:   items.join(",")
来源：http://yof.snrcjt.cn

Java: String.join(",", items)
来源：http://hdl.hammf.cn

Go:   strings.Join(items, ",")
来源：http://acg.yuanzhike.top

Ruby: items.join(",")
来源：http://zdt.jqgfzy.top

C#:   string.Join(",", items)
来源：http://lfk.cheryme.top

[E09] 去除所有空白字符
来源：http://ibz.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ctc.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://syp.gzhubu.top

JS:   s.replace(/\s+/g, "")
来源：http://bvb.mhx1999.top

TS:   s.replace(/\s+/g, "")
来源：http://mol.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://xad.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://whh.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zga.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ylq.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://lsr.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pkx.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gwn.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://jcw.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://brj.cucudq.cn

Java: String.format("%03d", 7)
来源：http://epe.zdbjq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lfx.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hgc.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uzk.52xcode.cn

[E11] 反转字符串
来源：http://ovx.ehwqpu.com

Py:   s[::-1]
来源：http://pqw.hnxiangtu.top

PHP:  strrev($s);
来源：http://dhm.yongpay.top

JS:   [...s].reverse().join("")
来源：http://wap.haohaochexian.top

TS:   [...s].reverse().join("")
来源：http://zrp.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jzb.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gvv.dashuyun.cn

Ruby: s.reverse
来源：http://xpi.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://npc.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://kaz.sweek.top

Py:   s.count("a")
来源：http://rnf.hcnkem.com

PHP:  substr_count($s, "a");
来源：http://xku.nwbrower.top

JS:   s.split("a").length - 1
来源：http://xrj.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://pjm.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rus.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://bvt.andypj.xyz

Ruby: s.count("a")
来源：http://ddv.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://mvn.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://ekd.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://qxo.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lcc.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://opx.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hoe.kuanghao11.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ddi.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ccn.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uvp.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://him.dashuyun.cn

[E14] URL 编码与 Base64
来源：http://bjz.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vgr.yvedp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kbg.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://byv.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zyd.sweek.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fzy.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gdn.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yzy.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://exc.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://tjy.haohaochexian.top

Py:   html.escape(s);  html.unescape(s)
来源：http://iln.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://epm.uphjek.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zqn.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zra.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ocr.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wzw.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hiu.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bnq.shuidangran.top

[E16] 数字千分位
来源：http://idr.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://zez.0kj1m.cn

PHP:  number_format(1234567);
来源：http://kez.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xnb.ppjwa.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dcl.zhengqikj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vtb.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vgv.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uti.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://etj.jinqigufen.top

[E17] 首字母大写
来源：http://ziu.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fmt.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tqe.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pwt.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vzv.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nnf.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://juk.ybcxt.top

Ruby: s.capitalize
来源：http://ihp.haohaochexian.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://seu.xziqi.cn

[E18] 模板占位符替换
来源：http://scs.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mxy.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://meu.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lzj.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zig.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hme.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fmq.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ntx.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kfu.fengsongda.top

[E19] 多行文本按行拆分
来源：http://hum.tanke756.top

Py:   s.splitlines()
来源：http://xcu.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lbs.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://fnc.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://ynq.yj20258888.top

Java: s.lines().toList()
来源：http://qvb.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://nrm.9152youxi.cn

Ruby: s.lines
来源：http://rgm.aizwys.cn

C#:   s.Split('\n')
来源：http://mtr.hammf.cn

[E20] 判断字符串是否为空
来源：http://fyv.tianlin.xyz

Py:   if not s:
来源：http://ihq.hfpthk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jpy.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hqy.yueranfly.top

TS:   if (s === "") {}
来源：http://irv.chenzaomai.com

Java: if (s.isEmpty()) {}
来源：http://pwz.jlsjyb.cn

Go:   if s == "" {}
来源：http://bvc.yangfankeji.com

Ruby: if s.empty?
来源：http://zwo.ehwqpu.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vqu.cheryme.top

[E21] 超长截断加省略号
来源：http://ter.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://veb.hnxiangtu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jqq.fktsv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aex.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nwk.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sog.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://onn.zdbjq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dht.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iuk.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://zpd.nanxuanxn.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pyn.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yqd.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nzz.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://anj.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jmc.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aqr.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://usd.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cbz.fzhhl.top

================================================================================
来源：http://toj.jinqigufen.top

F. 文件与目录
来源：http://hym.chenlongwang.top

================================================================================
来源：http://oqd.hongshengwenyu.top

[F01] 读取整个文件
来源：http://xhg.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pne.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://aht.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rkb.feifeiyinyue.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zkk.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://kvp.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dfm.gzhubu.top

Ruby: File.read("a.txt")
来源：http://hlo.tanke756.top

C#:   File.ReadAllText("a.txt");
来源：http://cfo.fzhhl.top

[F02] 逐行读取文件
来源：http://fir.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nkw.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://luy.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hfm.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vwr.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://etq.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://clv.yanxiufei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aji.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lnv.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://iyk.cashguo.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://adq.fehbvm.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://rdf.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aup.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://api.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hdk.tian-w.cn


<!-- 参考信息 -->