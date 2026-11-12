代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fpb.jinqigufen.top

Go:   // 手写双层循环
来源：http://nrj.fzhhl.top

Ruby: nested.flatten
来源：http://esk.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fur.yj20258888.top

[D19] 按字段分组
来源：http://vgs.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://khn.aizwys.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://urd.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tfq.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://odu.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rtq.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://mrn.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zfx.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ppu.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://rit.yj202588.top

Py:   Counter(arr)
来源：http://dqr.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://wkk.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qrm.nanxuanxn.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://avn.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xeo.epnwcf.com

Go:   // 手写 map[T]int
来源：http://jto.cashguo.top

Ruby: arr.tally
来源：http://vuq.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tkl.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://flq.hnxiangtu.top

Py:   x in arr
来源：http://nid.yonumen.top

PHP:  in_array($x, $arr, true);
来源：http://ibm.zhijiandao.cn

JS:   arr.includes(x)
来源：http://coq.zhoulong.xyz

TS:   arr.includes(x)
来源：http://exl.fengsongda.top

Java: list.contains(x)
来源：http://nxr.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://qdr.316326.xyz

Ruby: arr.include?(x)
来源：http://bgz.dashuyun.cn

C#:   list.Contains(x)
来源：http://uej.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://dao.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fkj.meibo888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vlm.ybcxt.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hjm.zhoulong.xyz

TS:   [...arr];
来源：http://lsx.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://ngx.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://jxz.tian-w.cn

Ruby: arr.dup;  arr.clone
来源：http://mid.sxryk.cn

C#:   new List<int>(list);
来源：http://fit.uphjek.com

[D23] reduce 累积计算
来源：http://hzx.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ciw.shzxlz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uua.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xtb.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pht.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rrz.hcnkem.com

Go:   // 手写循环
来源：http://fpo.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://put.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://doy.jinyuanbaomall.cn

[D24] 字典 / Map 基本操作
来源：http://sll.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rqu.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hts.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wfn.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lci.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ujx.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iab.vqdsnc.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wex.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rxy.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://jyj.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://udx.tian-w.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://paq.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ckb.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fek.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uon.hfpthk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://evx.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mjq.haohaochexian.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ryk.52xcode.cn

[D26] 数组转字符串
来源：http://lqx.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://mub.sysykeji.top

PHP:  implode(", ", $arr);
来源：http://zrb.havefunace.top

JS:   arr.join(", ")
来源：http://xaz.cheryme.top

TS:   arr.join(", ")
来源：http://kej.sjlbkw.cn

Java: String.join(", ", list)
来源：http://swa.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://rnj.cdnleiting.top

Ruby: arr.join(", ")
来源：http://fui.xylfe.cn

C#:   string.Join(", ", list)
来源：http://yvi.yuanzhike.top

================================================================================
来源：http://kdj.xuanzx.com

E. 字符串处理
来源：http://xua.jiagoushi.top

================================================================================
来源：http://csk.zhengqikj.top

[E01] 拼接字符串
来源：http://zhm.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://izj.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qke.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hkh.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cwt.sysykeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bix.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jkc.sufxvd.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zaq.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yms.52xcode.cn

[E02] 重复字符串
来源：http://pst.yfazqb.com

Py:   "ab" * 3
来源：http://skb.hongshengwenyu.top

PHP:  str_repeat("ab", 3);
来源：http://noa.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://bwl.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://hmq.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://cub.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://bip.vqdsnc.cn

Ruby: "ab" * 3
来源：http://lpr.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pwj.sjlbkw.cn

[E03] 截取子串
来源：http://zln.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://evd.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ayg.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rau.zhaomingkeji.xyz

TS:   s.slice(1, 4)
来源：http://vxh.cdnleiting.top

Java: s.substring(1, 4)
来源：http://gbs.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dzf.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://asi.yj20258.top

C#:   s.Substring(1, 3)
来源：http://ola.kuanghao11.cn

[E04] 查找子串位置
来源：http://kni.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://gly.gotoacloud.top

PHP:  strpos($s, "x");
来源：http://sfx.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kkz.dianchejie.cn

TS:   s.indexOf("x")
来源：http://mds.zhongyouzk.top

Java: s.indexOf("x")
来源：http://kvo.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://kgo.zhixingplan.top

Ruby: s.index("x")
来源：http://foj.bbcook.cn

C#:   s.IndexOf("x")
来源：http://cqt.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qmn.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bey.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zsv.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://egz.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ljg.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bdm.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ogq.yueranfly.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gyo.bbcook.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wts.nanxuanxn.top

[E06] 替换子串
来源：http://jeg.xuetiantiany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mmq.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://rpc.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gbm.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://yxz.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sjy.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lau.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lil.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://xmg.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://pco.ybcxt.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oqe.sjlbkw.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kze.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://gdj.wangshuangyany.cn

TS:   s.split(",")
来源：http://nvo.gaohongyu789.top

Java: s.split(",");  s.split("\\s+")
来源：http://wib.meibo888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uan.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://rkl.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nuy.meibo888.top

[E08] 数组按分隔符合并
来源：http://cbw.yj20258888.top

Py:   ",".join(items)
来源：http://bnf.cqqwz.cn

PHP:  implode(",", $items);
来源：http://pkf.hammf.cn

JS:   items.join(",")
来源：http://jge.zycfv.cn

TS:   items.join(",")
来源：http://hpw.fzhhl.top

Java: String.join(",", items)
来源：http://kdg.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://wjf.zhixingplan.top

Ruby: items.join(",")
来源：http://ogj.shuidangran.top

C#:   string.Join(",", items)
来源：http://mkv.havefunace.top

[E09] 去除所有空白字符
来源：http://ofc.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ein.hywenlv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pgy.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://urd.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://vcw.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://vrf.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jbx.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://edf.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://puw.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://qqo.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cjg.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qiw.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://fxb.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://bxw.hesvh.cn

Java: String.format("%03d", 7)
来源：http://shc.dianchejie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://phf.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ngm.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mht.sxryk.cn

[E11] 反转字符串
来源：http://daf.c1oappe.top

Py:   s[::-1]
来源：http://yzv.jiagoushi.top

PHP:  strrev($s);
来源：http://kbq.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://ttw.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://gip.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://isg.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hta.cashguo.top

Ruby: s.reverse
来源：http://tzq.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://hck.yueranfly.top

[E12] 统计某字符出现次数
来源：http://nwp.tianlin.xyz

Py:   s.count("a")
来源：http://kcf.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://ity.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://rhw.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://tup.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xmf.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://vqh.jianghu66.top

Ruby: s.count("a")
来源：http://igo.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://xbe.ydzc1.top

[E13] 逐字符遍历
来源：http://vbx.birdmap.top

Py:   for ch in s: print(ch)
来源：http://gtv.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ndw.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lvj.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://iit.tanke756.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lwt.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tdy.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ebv.zhongyouzk.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wvv.smart0.xyz

[E14] URL 编码与 Base64
来源：http://flj.hnqzz.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://llo.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://npn.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qfa.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vtf.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ixu.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lup.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vnv.shangyingyoupin.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dij.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://kan.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://eln.hammf.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vbi.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qks.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://mii.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ebx.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vcf.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pbk.jiagoushi.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nhm.wangdashe.top

[E16] 数字千分位
来源：http://aon.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://pwh.bbcook.cn

PHP:  number_format(1234567);
来源：http://vfa.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://arl.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dzn.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wod.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eon.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wnu.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://xnq.shuidangran.top

[E17] 首字母大写
来源：http://kzz.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://war.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iwk.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kmy.mhx1999.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gar.chenjidiqi.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xkk.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pph.daxiang520.top

Ruby: s.capitalize
来源：http://jsn.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cou.sweek.top

[E18] 模板占位符替换
来源：http://uez.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ywq.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nvf.fengsongda.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uel.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hzn.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kcr.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://djk.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qcv.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jhn.fzhhl.top

[E19] 多行文本按行拆分
来源：http://gib.ehwqpu.com

Py:   s.splitlines()
来源：http://mzp.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://goo.zhaomingkeji.xyz

JS:   s.split(/\r?\n/)
来源：http://ssi.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://spa.xuetiantiany.cn

Java: s.lines().toList()
来源：http://quh.hammf.cn

Go:   strings.Split(s, "\n")
来源：http://ajm.guowangkeji.top

Ruby: s.lines
来源：http://ukd.guannengcc.top

C#:   s.Split('\n')
来源：http://rhi.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://wom.chenjidiqi.icu

Py:   if not s:
来源：http://kxj.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cvj.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ikt.mhx1999.top

TS:   if (s === "") {}
来源：http://xbi.c1oappe.top

Java: if (s.isEmpty()) {}
来源：http://iun.zdqjudy.top

Go:   if s == "" {}
来源：http://frg.yuanzhike.top

Ruby: if s.empty?
来源：http://slc.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://psa.yonumen.top

[E21] 超长截断加省略号
来源：http://qwu.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hyv.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://egu.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gqf.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rdp.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nry.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://gdz.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://whb.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xhx.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://rmk.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yxp.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://phr.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ser.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hxa.aibaodan.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aec.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dpo.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://ula.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gvl.yangfankeji.com

================================================================================
来源：http://ezw.ppjwa.cn

F. 文件与目录
来源：http://jme.fengsongda.top

================================================================================
来源：http://iiu.guannengcc.top

[F01] 读取整个文件
来源：http://cmy.shzxlz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fbw.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://kje.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://krp.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://com.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xms.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eos.vqdsnc.cn

Ruby: File.read("a.txt")
来源：http://ryb.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://fcn.jqgfzy.top

[F02] 逐行读取文件
来源：http://bft.gaohongyu789.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wnw.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fgl.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://owb.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tdv.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ahq.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rqk.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mtw.wangdashe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uuw.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://xqm.jinghuilouyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gec.tianlin.xyz


<!-- 参考信息 -->