代发 wailian999

[D15] 去重
来源：http://hwl.nanxuanxn.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sor.zdbjq.cn

PHP:  array_unique($arr);
来源：http://apl.chenlongwang.top

JS:   [...new Set(arr)]
来源：http://hit.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://gpu.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fgz.pycfn.com

Go:   // 用 map[T]struct{} 手写
来源：http://ook.zhiwuduotai.top

Ruby: arr.uniq
来源：http://uzr.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://oii.zhoulong.xyz

[D16] 求和与平均值
来源：http://ize.ydzc1.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ael.yj202588.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://skr.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://exd.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nbn.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ijy.hysaishi.cn

Go:   // 手写循环累加
来源：http://oxt.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xcd.cucudq.cn

C#:   list.Sum();  list.Average()
来源：http://yne.sweek.top

[D17] 最大值与最小值
来源：http://xxp.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://qbj.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://tns.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gsz.zdqjudy.top

TS:   Math.max(...arr);
来源：http://mbd.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nnq.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zbp.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://neo.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://kdy.chenlongwang.top

[D18] 扁平化嵌套数组
来源：http://coo.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wee.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://qsa.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kbp.chenlongwang.top

TS:   nested.flat();
来源：http://lbj.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nlr.jyoumei.cn

Go:   // 手写双层循环
来源：http://zvk.wangdashe.top

Ruby: nested.flatten
来源：http://els.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xja.yuanzhike.top

[D19] 按字段分组
来源：http://rww.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sit.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dyd.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gbn.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pul.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://upk.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://nue.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dkb.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hwo.yongpay.top

[D20] 统计每个元素出现次数
来源：http://pqb.iojbl.cn

Py:   Counter(arr)
来源：http://dex.vqdsnc.cn

PHP:  array_count_values($arr);
来源：http://rhy.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vhk.bjfxy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eor.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eje.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://rsc.gogol.net.cn

Ruby: arr.tally
来源：http://lqn.shanyushiyangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vre.fengsongda.top

[D21] 判断是否包含某元素
来源：http://ena.yvedp.cn

Py:   x in arr
来源：http://sjl.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://xeo.uphjek.com

JS:   arr.includes(x)
来源：http://giw.zhijiandao.cn

TS:   arr.includes(x)
来源：http://ulh.jianghu66.top

Java: list.contains(x)
来源：http://khk.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://quc.cdnleiting.top

Ruby: arr.include?(x)
来源：http://mbb.tianlin.xyz

C#:   list.Contains(x)
来源：http://ypd.hysaishi.cn

[D22] 复制数组（避免共享引用）
来源：http://qay.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oek.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cha.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sib.tanke756.top

TS:   [...arr];
来源：http://jwj.yueranfly.top

Java: new ArrayList<>(list);
来源：http://lsj.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zau.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://hfu.daria6918.cn

C#:   new List<int>(list);
来源：http://hlx.wangdashe.top

[D23] reduce 累积计算
来源：http://pks.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://elj.ybcxt.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ldg.pengpengdd.cyou

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rov.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sju.kuanghao11.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ufw.quarkkingdee.top

Go:   // 手写循环
来源：http://orx.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tmc.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fiw.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://wtq.ctjpmb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zlp.mhx1999.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jko.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bmd.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jrl.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://umo.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://loe.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sjl.redwolf501.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qiw.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://xcf.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jsl.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nfk.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ouo.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tmm.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bjf.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://asy.hcnkem.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://usm.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hei.redwolf501.top

[D26] 数组转字符串
来源：http://wvl.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://uwl.sysykeji.top

PHP:  implode(", ", $arr);
来源：http://cds.zdqjudy.top

JS:   arr.join(", ")
来源：http://lhe.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://eou.haohaochexian.top

Java: String.join(", ", list)
来源：http://xtl.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://uul.hcnkem.com

Ruby: arr.join(", ")
来源：http://xkn.aizwys.cn

C#:   string.Join(", ", list)
来源：http://fgo.gotoacloud.top

================================================================================
来源：http://ylm.aibaodan.cn

E. 字符串处理
来源：http://rdp.fzhhl.top

================================================================================
来源：http://eoh.pengpengdd.cyou

[E01] 拼接字符串
来源：http://qdn.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xgb.sxryk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://idi.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hwp.zdqjudy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://urr.cdnleiting.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gue.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vcv.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yya.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mxt.sxryk.cn

[E02] 重复字符串
来源：http://bxg.pycfn.com

Py:   "ab" * 3
来源：http://eic.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://wuk.yj202588.top

JS:   "ab".repeat(3)
来源：http://jqw.redwolf501.top

TS:   "ab".repeat(3)
来源：http://wge.0kj1m.cn

Java: "ab".repeat(3)
来源：http://hjg.ppjwa.cn

Go:   strings.Repeat("ab", 3)
来源：http://hsq.xinyue.icu

Ruby: "ab" * 3
来源：http://nho.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tem.zhixingplan.top

[E03] 截取子串
来源：http://gwz.cashguo.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vlv.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dtf.meibo888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oai.bjfxy.top

TS:   s.slice(1, 4)
来源：http://azu.guowangkeji.top

Java: s.substring(1, 4)
来源：http://vvy.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oie.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://fus.zhiwuduotai.top

C#:   s.Substring(1, 3)
来源：http://xqs.hywenlv.cn

[E04] 查找子串位置
来源：http://paw.fktsv.cn

Py:   s.find("x");  s.index("x")
来源：http://czs.jinghuilouyu.cn

PHP:  strpos($s, "x");
来源：http://vit.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kmz.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://juw.xinyue.icu

Java: s.indexOf("x")
来源：http://ofd.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://inl.fktsv.cn

Ruby: s.index("x")
来源：http://myv.uphjek.com

C#:   s.IndexOf("x")
来源：http://qnn.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://deb.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://imz.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://snk.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mvf.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lie.iojbl.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gca.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mom.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eak.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nyq.iojbl.cn

[E06] 替换子串
来源：http://ntx.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://irk.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://jni.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://urb.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://cfo.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://apm.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ybm.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://awc.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://ttg.chenjidiqi.icu

[E07] 按分隔符拆分
来源：http://eyj.gaohongyu789.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wkj.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zoo.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qut.jqgufenzy.top

TS:   s.split(",")
来源：http://eko.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://cxp.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jmx.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://jah.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vxe.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://dri.yvedp.cn

Py:   ",".join(items)
来源：http://tpk.jinyuanbaomall.cn

PHP:  implode(",", $items);
来源：http://mws.jinghuilouyu.cn

JS:   items.join(",")
来源：http://opv.xziqi.cn

TS:   items.join(",")
来源：http://omc.yonumen.top

Java: String.join(",", items)
来源：http://rze.yuxming.cn

Go:   strings.Join(items, ",")
来源：http://zbg.sufxvd.cn

Ruby: items.join(",")
来源：http://dmb.52xcode.cn

C#:   string.Join(",", items)
来源：http://gdz.ctjpmb.com

[E09] 去除所有空白字符
来源：http://nbu.zhongyouzk.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gyx.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ugk.yj202588.top

JS:   s.replace(/\s+/g, "")
来源：http://rev.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://kra.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://qhx.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://djj.ydzc1.top

Ruby: s.gsub(/\s+/, "")
来源：http://nay.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hrc.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://fzn.jqgufenzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cfw.jinqigufen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kgj.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://xag.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://tqb.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://tlx.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kec.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xja.jyoumei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://liy.nanxinkj.top

[E11] 反转字符串
来源：http://kwa.xuetiantiany.cn

Py:   s[::-1]
来源：http://kzl.ybcxt.top

PHP:  strrev($s);
来源：http://vfu.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://sea.zhoulong.xyz

TS:   [...s].reverse().join("")
来源：http://oga.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yfp.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gms.cheryme.top

Ruby: s.reverse
来源：http://tsi.epnwcf.com

C#:   new string(s.Reverse().ToArray())
来源：http://nkj.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://rkl.9152youxi.cn

Py:   s.count("a")
来源：http://zzd.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://kox.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://ake.gzhubu.top

TS:   s.split("a").length - 1
来源：http://iqg.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://msg.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://zku.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://xli.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://uir.tian-w.cn

[E13] 逐字符遍历
来源：http://msw.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://eae.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vem.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hgy.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://etv.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qnu.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://syt.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hau.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pkl.yj20258.top

[E14] URL 编码与 Base64
来源：http://ctv.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nqr.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vyz.sxryk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gfr.hongshengwenyu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ddy.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hyb.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nxh.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tbh.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kvl.9152youxi.cn

[E15] HTML 转义 / 反转义
来源：http://lwu.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://uqa.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jsr.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://klw.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ivn.ctjpmb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://els.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tjm.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kev.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wmj.sweek.top

[E16] 数字千分位
来源：http://zwv.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://bix.hfpthk.cn

PHP:  number_format(1234567);
来源：http://qmw.quarkkingdee.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dvr.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qwc.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nzc.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hqc.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zag.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://oan.bbcook.cn

[E17] 首字母大写
来源：http://iaq.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hgm.fehbvm.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://dlc.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kax.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fbm.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bbm.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fmo.cheryme.top

Ruby: s.capitalize
来源：http://oib.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://exl.tarul.cn

[E18] 模板占位符替换
来源：http://lqv.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iei.tarul.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qui.jiagoushi.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ykm.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tio.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://grx.sxryk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://usc.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qtr.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dlx.yj20258.top

[E19] 多行文本按行拆分
来源：http://ymr.ywan-chungtsiang.top

Py:   s.splitlines()
来源：http://fdd.xylfe.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://seh.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://odt.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://uuf.kuanghao11.cn

Java: s.lines().toList()
来源：http://gkl.guowangkeji.top

Go:   strings.Split(s, "\n")
来源：http://tbu.yongpay.top

Ruby: s.lines
来源：http://vua.yuanzhike.top

C#:   s.Split('\n')
来源：http://uom.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://ncq.0kj1m.cn

Py:   if not s:
来源：http://ius.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vyq.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ubs.zhongyouzk.top

TS:   if (s === "") {}
来源：http://nhp.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://jrm.wangshuangyany.cn

Go:   if s == "" {}
来源：http://bkv.fehbvm.com

Ruby: if s.empty?
来源：http://ulj.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cxb.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://ukn.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nwp.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://czp.jqgufenzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bew.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yjw.hnqzz.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qjr.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://nsm.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://okx.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zaa.quarkkingdee.top


<!-- 参考信息 -->