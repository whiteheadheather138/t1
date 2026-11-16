代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hia.fanxiaobao.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kvt.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://yzc.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://add.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lti.hammf.cn

Ruby: arr.max;  arr.min
来源：http://put.sweek.top

C#:   list.Max();  list.Min()
来源：http://qpw.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://rfl.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zim.ivvv.top

PHP:  array_merge(...$nested);
来源：http://vsy.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zli.xuanzx.com

TS:   nested.flat();
来源：http://tlr.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zbl.tian-w.cn

Go:   // 手写双层循环
来源：http://jsl.ybcxt.top

Ruby: nested.flatten
来源：http://kwk.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hxd.tarul.cn

[D19] 按字段分组
来源：http://bvk.chenjidiqi.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gef.chenzaomai.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qwx.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xoq.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gbm.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zcn.zdqjudy.top

Go:   // 手写 map[string][]T
来源：http://krz.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fyc.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jkt.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://rmj.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://lmd.zhijiandao.cn

PHP:  array_count_values($arr);
来源：http://upn.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vvm.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://owl.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rwt.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://mjl.shuidangran.top

Ruby: arr.tally
来源：http://qpm.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jha.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://pyy.jianghu66.top

Py:   x in arr
来源：http://nxz.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://kky.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://pxy.xuetiantiany.cn

TS:   arr.includes(x)
来源：http://sxx.tarul.cn

Java: list.contains(x)
来源：http://uee.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://fzp.yj20258.top

Ruby: arr.include?(x)
来源：http://dqk.tianlin.xyz

C#:   list.Contains(x)
来源：http://vcd.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://yhc.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gus.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://esk.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mer.pengpengdd.cyou

TS:   [...arr];
来源：http://owz.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://jox.jiagoushi.top

Go:   copied := append([]int(nil), arr...)
来源：http://ykl.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://xra.xziqi.cn

C#:   new List<int>(list);
来源：http://gta.wangdashe.top

[D23] reduce 累积计算
来源：http://xdc.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pvl.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ujj.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hkh.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nea.guannengcc.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zey.tianlin.xyz

Go:   // 手写循环
来源：http://vmu.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vhb.zhoulong.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qtt.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://buy.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zvc.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oiy.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fok.andypj.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://edw.ydzc1.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mlu.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://stl.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://msh.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cmx.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://doe.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ajl.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wbg.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ury.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xpt.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mhx.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gxl.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yxm.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dpa.cheryme.top

[D26] 数组转字符串
来源：http://clv.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://vym.uphjek.com

PHP:  implode(", ", $arr);
来源：http://xkx.tarul.cn

JS:   arr.join(", ")
来源：http://fev.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://kwx.xylfe.cn

Java: String.join(", ", list)
来源：http://fpi.ydjk.org.cn

Go:   strings.Join(strs, ", ")
来源：http://sah.shuidangran.top

Ruby: arr.join(", ")
来源：http://xnj.cdnleiting.top

C#:   string.Join(", ", list)
来源：http://fms.chenzaomai.com

================================================================================
来源：http://gzq.nwbrower.top

E. 字符串处理
来源：http://xlw.smart0.xyz

================================================================================
来源：http://nlv.chenjidiqi.icu

[E01] 拼接字符串
来源：http://tpe.ywan-chungtsiang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://opb.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rxw.yfazqb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://syf.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bib.feifeiyinyue.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lru.cdnleiting.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qjc.guannengcc.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pne.jlsjyb.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jby.fzhhl.top

[E02] 重复字符串
来源：http://nwl.chenjidiqi.icu

Py:   "ab" * 3
来源：http://zgz.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://sat.birdmap.top

JS:   "ab".repeat(3)
来源：http://sni.tarul.cn

TS:   "ab".repeat(3)
来源：http://jvf.birdmap.top

Java: "ab".repeat(3)
来源：http://ssh.wangdashe.top

Go:   strings.Repeat("ab", 3)
来源：http://vyj.jinqigufen.top

Ruby: "ab" * 3
来源：http://lxo.cqqwz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://byo.aibaodan.cn

[E03] 截取子串
来源：http://jfp.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kgc.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xwq.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jbz.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://txf.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://mpi.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uht.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://oln.ivvv.top

C#:   s.Substring(1, 3)
来源：http://ezl.jyoumei.cn

[E04] 查找子串位置
来源：http://gjs.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://axp.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://mon.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uge.yj20258.top

TS:   s.indexOf("x")
来源：http://wpd.chenzaomai.com

Java: s.indexOf("x")
来源：http://jje.hammf.cn

Go:   strings.Index(s, "x")
来源：http://ydf.tian-w.cn

Ruby: s.index("x")
来源：http://yvk.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://eha.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://svr.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zns.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://imu.daxiang520.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jdf.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fnd.xingfuxueyuan.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wql.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hyd.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lal.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yjj.yuanzhike.top

[E06] 替换子串
来源：http://aeh.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://idu.sysykeji.top

PHP:  str_replace("a", "b", $s);
来源：http://pwz.aibaodan.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dqv.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://wuz.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hej.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lpi.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ung.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://kwd.yj202588.top

[E07] 按分隔符拆分
来源：http://hhj.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hlk.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ujf.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://shm.pengpengdd.cyou

TS:   s.split(",")
来源：http://wsl.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://uzx.redwolf501.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zqr.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://sey.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://itk.cheryme.top

[E08] 数组按分隔符合并
来源：http://pbt.uphjek.com

Py:   ",".join(items)
来源：http://bhb.jqgfzy.top

PHP:  implode(",", $items);
来源：http://gzs.yfazqb.com

JS:   items.join(",")
来源：http://phf.52xcode.cn

TS:   items.join(",")
来源：http://trq.ctjpmb.com

Java: String.join(",", items)
来源：http://ypn.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://cmu.vehdjk.com

Ruby: items.join(",")
来源：http://dic.gogol.net.cn

C#:   string.Join(",", items)
来源：http://ddz.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://vyj.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zqm.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ifm.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://vdn.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://use.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://xvd.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gsl.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://byw.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jtz.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://dxl.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lfq.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wck.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://gbo.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://fml.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://iqc.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://yrq.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://csr.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hcb.vqdsnc.cn

[E11] 反转字符串
来源：http://car.cheryme.top

Py:   s[::-1]
来源：http://zmw.vqdsnc.cn

PHP:  strrev($s);
来源：http://twd.gogol.net.cn

JS:   [...s].reverse().join("")
来源：http://xmr.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://vrz.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yqn.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mof.gogol.net.cn

Ruby: s.reverse
来源：http://ety.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://bcv.pengpengdd.cyou

[E12] 统计某字符出现次数
来源：http://xxe.nanxuanxn.top

Py:   s.count("a")
来源：http://tzm.316326.xyz

PHP:  substr_count($s, "a");
来源：http://prl.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://xxb.xuanzx.com

TS:   s.split("a").length - 1
来源：http://hru.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nhc.sweek.top

Go:   strings.Count(s, "a")
来源：http://qxn.feifeiyinyue.top

Ruby: s.count("a")
来源：http://xbj.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://hhu.zhijiandao.cn

[E13] 逐字符遍历
来源：http://coi.chenjidiqi.icu

Py:   for ch in s: print(ch)
来源：http://rqi.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oow.zdqjudy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://eic.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://itj.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yux.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bpg.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sqc.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xnk.pycfn.com

[E14] URL 编码与 Base64
来源：http://mbg.cucudq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://omq.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yua.jinqigufen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pfl.fanxiaobao.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mca.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://obg.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sqc.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gcm.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bro.ydjk.org.cn

[E15] HTML 转义 / 反转义
来源：http://tfm.zdqjudy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://iam.hnxiangtu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cki.zhongyouzk.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jtc.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qzd.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qkx.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ace.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pfe.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uut.xylfe.cn

[E16] 数字千分位
来源：http://ptn.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://eif.cucudq.cn

PHP:  number_format(1234567);
来源：http://fjp.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://asa.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pfb.xuanzx.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://swe.cdnleiting.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fax.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xay.shzxlz.cn

C#:   1234567.ToString("N0")
来源：http://hpa.guannengcc.top

[E17] 首字母大写
来源：http://swl.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bny.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://idf.yongpay.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bzi.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bfn.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xgb.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://coa.daria6918.cn

Ruby: s.capitalize
来源：http://hhp.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fws.nwbrower.top

[E18] 模板占位符替换
来源：http://pwh.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xho.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nis.uphjek.com

JS:   tpl.replaceAll("{name}", name)
来源：http://lnm.zhaomingkeji.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://cni.jiagoushi.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fji.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fhu.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xjp.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wrg.bjfxy.top

[E19] 多行文本按行拆分
来源：http://dka.tian-w.cn

Py:   s.splitlines()
来源：http://boe.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mdm.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://qnn.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://uzy.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://dot.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://vjb.zhoulong.xyz

Ruby: s.lines
来源：http://fvd.sjlbkw.cn

C#:   s.Split('\n')
来源：http://coo.epnwcf.com

[E20] 判断字符串是否为空
来源：http://npc.hammf.cn

Py:   if not s:
来源：http://ydn.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://huc.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://npn.316326.xyz

TS:   if (s === "") {}
来源：http://isb.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://qqc.gotoacloud.top

Go:   if s == "" {}
来源：http://xps.nanxuanxn.top

Ruby: if s.empty?
来源：http://coi.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pow.ppjwa.cn

[E21] 超长截断加省略号
来源：http://kld.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yzx.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mhc.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ztd.daria6918.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xyt.yvedp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zxz.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://rwf.ydjk.org.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bqv.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kxj.smart0.xyz

[E22] 字节长度与字符长度
来源：http://ubf.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uzx.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ljt.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lnf.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oqm.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yfj.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gnh.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://yys.ybcxt.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jvm.zhixingplan.top

================================================================================
来源：http://oba.0kj1m.cn

F. 文件与目录
来源：http://rut.yonumen.top

================================================================================
来源：http://rtg.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://myo.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://def.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://dsr.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://efy.hnxiangtu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://czw.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xcq.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rmv.hcnkem.com

Ruby: File.read("a.txt")
来源：http://xca.aizwys.cn


<!-- 参考信息 -->