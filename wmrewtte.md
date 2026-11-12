代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xze.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mvc.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vmo.yanxiufei.cn

Go:   // 手写循环累加
来源：http://fhz.daria6918.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tgh.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://mwo.daria6918.cn

[D17] 最大值与最小值
来源：http://yjy.havefunace.top

Py:   max(arr);  min(arr)
来源：http://otk.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://yta.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ocu.0kj1m.cn

TS:   Math.max(...arr);
来源：http://qtc.vqdsnc.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://usj.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ogi.uphjek.com

Ruby: arr.max;  arr.min
来源：http://qrg.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://fkg.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://jwd.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pgg.meibo888.top

PHP:  array_merge(...$nested);
来源：http://hja.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ctn.chenjidiqi.icu

TS:   nested.flat();
来源：http://ksu.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://aso.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://ael.fzhhl.top

Ruby: nested.flatten
来源：http://cxd.wangshuangyany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dov.aizwys.cn

[D19] 按字段分组
来源：http://vgn.smart0.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://txh.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tau.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xwn.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sup.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jum.yfazqb.com

Go:   // 手写 map[string][]T
来源：http://mkn.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ncb.shanyushiyangtech.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aca.ehwqpu.com

[D20] 统计每个元素出现次数
来源：http://jqh.jinqigufen.top

Py:   Counter(arr)
来源：http://lae.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://nqi.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tqi.cdnleiting.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vtx.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fgw.hcnkem.com

Go:   // 手写 map[T]int
来源：http://yrs.svipenyu.cn

Ruby: arr.tally
来源：http://fkd.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ikf.daxiang520.top

[D21] 判断是否包含某元素
来源：http://snj.hongshengwenyu.top

Py:   x in arr
来源：http://yft.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://add.pycfn.com

JS:   arr.includes(x)
来源：http://sqc.chenzaomai.com

TS:   arr.includes(x)
来源：http://geu.bjfxy.top

Java: list.contains(x)
来源：http://ypg.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://sgr.tianlin.xyz

Ruby: arr.include?(x)
来源：http://jhm.xylfe.cn

C#:   list.Contains(x)
来源：http://qxj.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://ndg.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fze.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yfg.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zbl.zhoulong.xyz

TS:   [...arr];
来源：http://vsp.birdmap.top

Java: new ArrayList<>(list);
来源：http://ggl.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://plc.fzhhl.top

Ruby: arr.dup;  arr.clone
来源：http://hdy.birdmap.top

C#:   new List<int>(list);
来源：http://fzg.ybcxt.top

[D23] reduce 累积计算
来源：http://vgz.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dtv.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zsz.kuanghao11.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yaf.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dab.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ima.hnqzz.top

Go:   // 手写循环
来源：http://ria.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kjr.zhaomingkeji.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fai.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://hlg.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kuv.zycfv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wuf.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wju.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zrr.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://boq.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://duw.cashguo.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blq.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qho.fehbvm.com

[D25] Set 集合去重与交并差
来源：http://qag.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tmu.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://stl.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zoh.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zdr.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://szz.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ppt.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://emm.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ofc.yuanzhike.top

[D26] 数组转字符串
来源：http://ezj.fehbvm.com

Py:   ", ".join(map(str, arr))
来源：http://xye.cucudq.cn

PHP:  implode(", ", $arr);
来源：http://uma.yangfankeji.com

JS:   arr.join(", ")
来源：http://fqe.ydjk.org.cn

TS:   arr.join(", ")
来源：http://she.jiagoushi.top

Java: String.join(", ", list)
来源：http://kge.shuidangran.top

Go:   strings.Join(strs, ", ")
来源：http://pda.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://rir.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://yqr.shanyushiyangtech.top

================================================================================
来源：http://iel.ehwqpu.com

E. 字符串处理
来源：http://vaj.birdmap.top

================================================================================
来源：http://aba.52xcode.cn

[E01] 拼接字符串
来源：http://vzj.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://etr.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rxk.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ept.shanyushiyangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sex.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hbs.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://his.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ant.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://haa.fengsongda.top

[E02] 重复字符串
来源：http://mtn.yj20258888.top

Py:   "ab" * 3
来源：http://tkt.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://sxi.daria6918.cn

JS:   "ab".repeat(3)
来源：http://fss.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://ywo.vehdjk.com

Java: "ab".repeat(3)
来源：http://gjp.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://nsh.meibo888.top

Ruby: "ab" * 3
来源：http://zlr.fehbvm.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://efv.nanxuanxn.top

[E03] 截取子串
来源：http://pwl.tianlin.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qjb.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mwn.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://boy.tanke756.top

TS:   s.slice(1, 4)
来源：http://wtk.jiagoushi.top

Java: s.substring(1, 4)
来源：http://pgq.pengpengdd.cyou

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://loi.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ygo.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://yvw.sufxvd.cn

[E04] 查找子串位置
来源：http://fvk.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://bol.uphjek.com

PHP:  strpos($s, "x");
来源：http://fiv.kuanghao11.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jcv.9152youxi.cn

TS:   s.indexOf("x")
来源：http://qnb.zdbjq.cn

Java: s.indexOf("x")
来源：http://dcx.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://lxa.chenzaomai.com

Ruby: s.index("x")
来源：http://lya.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://itk.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iwn.smart0.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gqt.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://use.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ofm.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://llz.svipenyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://knw.guannengcc.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qxw.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ryq.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mqw.hysaishi.cn

[E06] 替换子串
来源：http://xdj.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ion.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://gbf.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://phe.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://loj.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fyy.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bhs.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ais.shangyingyoupin.top

C#:   s.Replace("a", "b")
来源：http://qxo.ywan-chungtsiang.top

[E07] 按分隔符拆分
来源：http://esx.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wzm.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fcn.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://icr.ybcxt.top

TS:   s.split(",")
来源：http://zsq.birdmap.top

Java: s.split(",");  s.split("\\s+")
来源：http://uhi.nwbrower.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rlz.yuxming.cn

Ruby: s.split(",");  s.split
来源：http://kqa.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bmq.yueranfly.top

[E08] 数组按分隔符合并
来源：http://ehm.aizwys.cn

Py:   ",".join(items)
来源：http://dqi.haohaochexian.top

PHP:  implode(",", $items);
来源：http://amn.kuanghao11.cn

JS:   items.join(",")
来源：http://lqi.hysaishi.cn

TS:   items.join(",")
来源：http://mgs.ivvv.top

Java: String.join(",", items)
来源：http://idu.jiagoushi.top

Go:   strings.Join(items, ",")
来源：http://tat.bjfxy.top

Ruby: items.join(",")
来源：http://taz.zhiwuduotai.top

C#:   string.Join(",", items)
来源：http://bwo.guowangkeji.top

[E09] 去除所有空白字符
来源：http://wid.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xlb.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://and.tianlin.xyz

JS:   s.replace(/\s+/g, "")
来源：http://gxp.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://tyf.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://evq.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://ssw.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://ioz.jiagoushi.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ssx.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://xkd.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zfh.zhixingplan.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cra.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://cur.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://rnm.havefunace.top

Java: String.format("%03d", 7)
来源：http://jpi.svipenyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xsm.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yzc.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nwl.nwbrower.top

[E11] 反转字符串
来源：http://pjk.9152youxi.cn

Py:   s[::-1]
来源：http://gpu.shanyushiyangtech.top

PHP:  strrev($s);
来源：http://avq.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://ckd.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://iwq.pengpengdd.cyou

Java: new StringBuilder(s).reverse().toString()
来源：http://fol.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xkz.tian-w.cn

Ruby: s.reverse
来源：http://kcm.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://ixs.daria6918.cn

[E12] 统计某字符出现次数
来源：http://hck.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://jvj.cucudq.cn

PHP:  substr_count($s, "a");
来源：http://euv.andypj.xyz

JS:   s.split("a").length - 1
来源：http://ltr.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://rdq.jinghuilouyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jmz.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://qvt.chenlongwang.top

Ruby: s.count("a")
来源：http://fwc.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://avz.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://rbw.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://ron.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rau.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bxt.jqgfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://iti.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vgp.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uou.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nbx.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hlc.epnwcf.com

[E14] URL 编码与 Base64
来源：http://mja.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gqu.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ecg.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://soo.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pch.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zux.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://scc.fktsv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iyp.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zwq.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://vyi.fengsongda.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eba.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vlq.hywenlv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vmm.jinghuilouyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lll.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zto.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eyb.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ayw.316326.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mec.zhengqikj.top

[E16] 数字千分位
来源：http://xjz.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://ppk.zhixingplan.top

PHP:  number_format(1234567);
来源：http://bxw.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rwm.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://foj.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pby.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eep.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tgt.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://yqc.zdbjq.cn

[E17] 首字母大写
来源：http://ren.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rtk.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yrw.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jno.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://enb.jinyuanbaomall.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://opf.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fhp.uphjek.com

Ruby: s.capitalize
来源：http://cws.sysykeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tco.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://fmo.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zdb.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qox.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://jxm.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://lwb.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pyw.ppjwa.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://acy.guannengcc.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oox.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gsh.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://kip.chenzaomai.com

Py:   s.splitlines()
来源：http://drq.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hfs.smart0.xyz

JS:   s.split(/\r?\n/)
来源：http://xfw.cdnleiting.top

TS:   s.split(/\r?\n/)
来源：http://nhm.0kj1m.cn

Java: s.lines().toList()
来源：http://dcb.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://ago.fzhhl.top

Ruby: s.lines
来源：http://owu.shzxlz.cn

C#:   s.Split('\n')
来源：http://tti.guowangkeji.top

[E20] 判断字符串是否为空
来源：http://ujz.uphjek.com

Py:   if not s:
来源：http://ycs.yongpay.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yjv.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wzu.jqgfzy.top

TS:   if (s === "") {}
来源：http://hcs.cucudq.cn

Java: if (s.isEmpty()) {}
来源：http://rfp.iojbl.cn

Go:   if s == "" {}
来源：http://wri.wangdashe.top

Ruby: if s.empty?
来源：http://wps.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://npt.fktsv.cn

[E21] 超长截断加省略号
来源：http://vyw.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cvq.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tys.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://arm.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eaw.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://crh.xuanzx.com

Go:   // 按 rune 判断长度后截断
来源：http://gwq.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bkb.vehdjk.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iof.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://jim.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jcc.yj202588.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bcw.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dzl.pycfn.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dbj.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ynj.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jdd.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://ctn.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cny.shangyingyoupin.top

================================================================================
来源：http://uid.daria6918.cn

F. 文件与目录
来源：http://wue.tarul.cn

================================================================================
来源：http://trc.havefunace.top


<!-- 参考信息 -->