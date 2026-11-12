代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tsq.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://ccw.guannengcc.top

Ruby: nested.flatten
来源：http://vui.jqgfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rpp.zhengqikj.top

[D19] 按字段分组
来源：http://thm.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kau.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pyh.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ubn.yonumen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xux.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://neq.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://rbl.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ayn.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kpj.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://jka.tanke756.top

Py:   Counter(arr)
来源：http://pyo.ywan-chungtsiang.top

PHP:  array_count_values($arr);
来源：http://acn.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xgq.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lna.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pkc.9152youxi.cn

Go:   // 手写 map[T]int
来源：http://ogu.jqgufenzy.top

Ruby: arr.tally
来源：http://cwc.fengsongda.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kex.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://fre.zdqjudy.top

Py:   x in arr
来源：http://cpr.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://odv.zhixingplan.top

JS:   arr.includes(x)
来源：http://mau.jqgufenzy.top

TS:   arr.includes(x)
来源：http://rkw.sweek.top

Java: list.contains(x)
来源：http://qix.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://lxp.fengsongda.top

Ruby: arr.include?(x)
来源：http://gtr.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://asa.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://vqv.bbcook.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://coy.xingfuxueyuan.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://scu.shangyingyoupin.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aic.tian-w.cn

TS:   [...arr];
来源：http://vav.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://oog.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://osa.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://mhu.dashuyun.cn

C#:   new List<int>(list);
来源：http://fvk.yangfankeji.com

[D23] reduce 累积计算
来源：http://rxm.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ygn.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nxd.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jsj.daria6918.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://afr.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lsm.yangfankeji.com

Go:   // 手写循环
来源：http://bwu.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://edm.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mqe.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://sna.jiagoushi.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dyc.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xwl.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pcv.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sct.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wec.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xcu.cheryme.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ram.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yxg.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://ahb.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tot.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fjt.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://imo.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://glg.jyoumei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://unh.zhaomingkeji.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://boe.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jwn.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lce.hammf.cn

[D26] 数组转字符串
来源：http://iiq.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://jmn.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://bmt.gogol.net.cn

JS:   arr.join(", ")
来源：http://ams.gotoacloud.top

TS:   arr.join(", ")
来源：http://rpr.cucudq.cn

Java: String.join(", ", list)
来源：http://jbp.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://dvu.wangshuangyany.cn

Ruby: arr.join(", ")
来源：http://irc.daria6918.cn

C#:   string.Join(", ", list)
来源：http://jcj.hnqzz.top

================================================================================
来源：http://osx.jlsjyb.cn

E. 字符串处理
来源：http://rnq.feifeiyinyue.top

================================================================================
来源：http://hmp.bbcook.cn

[E01] 拼接字符串
来源：http://orw.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://teh.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kdy.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://byk.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://svf.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mfp.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ypv.cheryme.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yao.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dkh.0kj1m.cn

[E02] 重复字符串
来源：http://dxv.c1oappe.top

Py:   "ab" * 3
来源：http://qez.yvedp.cn

PHP:  str_repeat("ab", 3);
来源：http://nra.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://ika.quarkkingdee.top

TS:   "ab".repeat(3)
来源：http://zvk.fktsv.cn

Java: "ab".repeat(3)
来源：http://yku.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://jcp.guannengcc.top

Ruby: "ab" * 3
来源：http://iqx.yonumen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qkr.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://qaa.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bjl.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gzx.sweek.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tfa.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://tco.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://dtt.meibo888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hdv.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xhi.cashguo.top

C#:   s.Substring(1, 3)
来源：http://poy.cqqwz.cn

[E04] 查找子串位置
来源：http://lab.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://uum.xziqi.cn

PHP:  strpos($s, "x");
来源：http://aeh.birdmap.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mwu.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://jgk.fanxiaobao.xyz

Java: s.indexOf("x")
来源：http://xye.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://jcd.daxiang520.top

Ruby: s.index("x")
来源：http://vqi.smart0.xyz

C#:   s.IndexOf("x")
来源：http://fkl.fzhhl.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kaa.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dgh.wangdashe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tym.gogol.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ewb.sysykeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vat.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hco.xziqi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wbp.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nyx.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tvm.zhaomingkeji.xyz

[E06] 替换子串
来源：http://xoj.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://veg.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://lti.chenjidiqi.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mvs.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://zkh.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ozb.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cft.shangyingyoupin.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lbf.chenzaomai.com

C#:   s.Replace("a", "b")
来源：http://xvy.jinghuilouyu.cn

[E07] 按分隔符拆分
来源：http://dly.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mku.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qzq.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://puh.yj20258.top

TS:   s.split(",")
来源：http://ujn.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vox.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://arq.cashguo.top

Ruby: s.split(",");  s.split
来源：http://usv.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lym.aizwys.cn

[E08] 数组按分隔符合并
来源：http://kbk.dashuyun.cn

Py:   ",".join(items)
来源：http://ime.yj20258888.top

PHP:  implode(",", $items);
来源：http://tvx.tianlin.xyz

JS:   items.join(",")
来源：http://mub.jlsjyb.cn

TS:   items.join(",")
来源：http://dpq.hnqzz.top

Java: String.join(",", items)
来源：http://umq.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://szn.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://yiv.pycfn.com

C#:   string.Join(",", items)
来源：http://teq.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://dze.zdbjq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://txu.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qvv.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://pbv.gotoacloud.top

TS:   s.replace(/\s+/g, "")
来源：http://pdo.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://dbl.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://sgs.yangfankeji.com

Ruby: s.gsub(/\s+/, "")
来源：http://zpq.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jxz.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://iis.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://upu.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cgy.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://ubp.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://ruu.yj20258.top

Java: String.format("%03d", 7)
来源：http://cud.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://hqe.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ujp.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xfe.guannengcc.top

[E11] 反转字符串
来源：http://erj.hongshengwenyu.top

Py:   s[::-1]
来源：http://bkn.sxryk.cn

PHP:  strrev($s);
来源：http://pgv.yuxming.cn

JS:   [...s].reverse().join("")
来源：http://yxg.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://mfn.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uzz.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ogi.jinqigfzy.top

Ruby: s.reverse
来源：http://wuf.vehdjk.com

C#:   new string(s.Reverse().ToArray())
来源：http://bnr.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://hfv.mhx1999.top

Py:   s.count("a")
来源：http://fcx.cucudq.cn

PHP:  substr_count($s, "a");
来源：http://frm.316326.xyz

JS:   s.split("a").length - 1
来源：http://ocj.ppjwa.cn

TS:   s.split("a").length - 1
来源：http://ysl.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tse.ppjwa.cn

Go:   strings.Count(s, "a")
来源：http://fug.zhijiandao.cn

Ruby: s.count("a")
来源：http://bxn.redwolf501.top

C#:   s.Count(c => c == 'a')
来源：http://sfn.cheryme.top

[E13] 逐字符遍历
来源：http://gkh.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://gqe.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lsq.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://uae.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dfs.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yho.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lhi.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wxp.sweek.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ppg.ehwqpu.com

[E14] URL 编码与 Base64
来源：http://vvu.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://grd.sweek.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nda.ybcxt.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rrv.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wig.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eur.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tqc.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hws.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yoo.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://wxr.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hxm.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pka.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jtq.zhixingplan.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dlh.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aiz.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ovo.bbcook.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gnc.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cee.316326.xyz

[E16] 数字千分位
来源：http://yfd.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://fsz.yonumen.top

PHP:  number_format(1234567);
来源：http://kwi.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://iip.shuidangran.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zak.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sqr.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iye.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bno.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://fxw.tanke756.top

[E17] 首字母大写
来源：http://uoj.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bhv.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://puf.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aba.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://igv.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ytc.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lcz.shzxlz.cn

Ruby: s.capitalize
来源：http://umx.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eyf.zycfv.cn

[E18] 模板占位符替换
来源：http://stl.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ung.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gwy.jqgfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://akc.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://aja.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://njo.fanxiaobao.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://enb.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hkn.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gyg.tian-w.cn

[E19] 多行文本按行拆分
来源：http://bni.pycfn.com

Py:   s.splitlines()
来源：http://jfk.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://err.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://apm.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://rfg.cucudq.cn

Java: s.lines().toList()
来源：http://yql.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://npa.yuanzhike.top

Ruby: s.lines
来源：http://jvm.yangfankeji.com

C#:   s.Split('\n')
来源：http://ulw.sxryk.cn

[E20] 判断字符串是否为空
来源：http://fqd.hysaishi.cn

Py:   if not s:
来源：http://vpf.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ofl.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zbo.tianlin.xyz

TS:   if (s === "") {}
来源：http://xul.havefunace.top

Java: if (s.isEmpty()) {}
来源：http://qmj.cashguo.top

Go:   if s == "" {}
来源：http://dim.zhixingplan.top

Ruby: if s.empty?
来源：http://tor.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ego.smart0.xyz

[E21] 超长截断加省略号
来源：http://koj.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ehr.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://erk.meibo888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oxq.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mbd.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rej.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://gez.nanxuanxn.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eox.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hgx.yongpay.top

[E22] 字节长度与字符长度
来源：http://jur.cheryme.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://suw.ivvv.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ywb.tarul.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://amj.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dvi.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gvi.wangshuangyany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fak.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://sro.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oqz.hammf.cn

================================================================================
来源：http://sib.wangshuangyany.cn

F. 文件与目录
来源：http://gsi.yj202588.top

================================================================================
来源：http://bgh.yfazqb.com

[F01] 读取整个文件
来源：http://lpr.fanxiaobao.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ssn.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://lxq.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uca.yueranfly.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rrz.jinqigufen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zoo.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gza.cashguo.top

Ruby: File.read("a.txt")
来源：http://sec.hnqzz.top

C#:   File.ReadAllText("a.txt");
来源：http://cdf.yuxming.cn

[F02] 逐行读取文件
来源：http://jul.sjlbkw.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zmy.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qqn.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ujg.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hdi.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://swj.yuanzhike.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://djf.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jal.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qvr.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://vjm.haohaochexian.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oze.uphjek.com


<!-- 参考信息 -->