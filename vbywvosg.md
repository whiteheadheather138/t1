代发 wailian999

TS:   [...new Set(arr)]
来源：http://sck.zhengqikj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jnl.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://crc.chenlongwang.top

Ruby: arr.uniq
来源：http://boh.uphjek.com

C#:   list.Distinct().ToList()
来源：http://idt.zdbjq.cn

[D16] 求和与平均值
来源：http://bga.jqgfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dfh.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rue.aizwys.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwu.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vhx.mhx1999.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aie.tanke756.top

Go:   // 手写循环累加
来源：http://uzn.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pbh.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://tuc.yfazqb.com

[D17] 最大值与最小值
来源：http://wsd.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://ejw.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://yjh.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jxj.bjfxy.top

TS:   Math.max(...arr);
来源：http://orv.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://eii.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kvt.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://lll.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://jyr.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://pgk.yj20258888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sul.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://zds.gaohongyu789.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tng.fehbvm.com

TS:   nested.flat();
来源：http://xzz.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cdd.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://dgq.birdmap.top

Ruby: nested.flatten
来源：http://izd.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bys.ehwqpu.com

[D19] 按字段分组
来源：http://orb.gogol.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mhg.bbcook.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gbt.xylfe.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xsz.hesvh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hhq.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nwt.chenlongwang.top

Go:   // 手写 map[string][]T
来源：http://dal.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://auq.cashguo.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rfi.zhoulong.xyz

[D20] 统计每个元素出现次数
来源：http://ccx.sufxvd.cn

Py:   Counter(arr)
来源：http://zek.nanxinkj.top

PHP:  array_count_values($arr);
来源：http://whk.chenzaomai.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eqq.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dyx.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ibv.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://blr.gaohongyu789.top

Ruby: arr.tally
来源：http://cxk.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qqa.birdmap.top

[D21] 判断是否包含某元素
来源：http://uzm.jinqigufen.top

Py:   x in arr
来源：http://nnl.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://xxe.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://pqw.smart0.xyz

TS:   arr.includes(x)
来源：http://hzj.52xcode.cn

Java: list.contains(x)
来源：http://ltx.jinqigfzy.top

Go:   slices.Contains(arr, x)
来源：http://ovz.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://udf.jinqigufen.top

C#:   list.Contains(x)
来源：http://lsy.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://brb.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kjk.quarkkingdee.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dtx.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iby.yangfankeji.com

TS:   [...arr];
来源：http://jjl.sxryk.cn

Java: new ArrayList<>(list);
来源：http://fxl.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://sga.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://mfo.fehbvm.com

C#:   new List<int>(list);
来源：http://sce.ehwqpu.com

[D23] reduce 累积计算
来源：http://nam.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://upo.kuanghao11.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rdo.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hzz.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ufw.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ckf.daria6918.cn

Go:   // 手写循环
来源：http://lfa.shzxlz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jbj.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dsk.xylfe.cn

[D24] 字典 / Map 基本操作
来源：http://qpz.yj20258888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xhy.sysykeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ctw.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vdh.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wpf.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rvf.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wtv.sweek.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mlx.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lxo.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://vag.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uil.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qtu.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://psd.vqdsnc.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jau.tianlin.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://caa.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kwn.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zbt.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://owu.dianchejie.cn

[D26] 数组转字符串
来源：http://hfw.jinghuilouyu.cn

Py:   ", ".join(map(str, arr))
来源：http://pur.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://tmf.tarul.cn

JS:   arr.join(", ")
来源：http://dxv.aibaodan.cn

TS:   arr.join(", ")
来源：http://drm.ehwqpu.com

Java: String.join(", ", list)
来源：http://rda.shuidangran.top

Go:   strings.Join(strs, ", ")
来源：http://nxd.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://ktw.c1oappe.top

C#:   string.Join(", ", list)
来源：http://tbl.feifeiyinyue.top

================================================================================
来源：http://krk.xuanzx.com

E. 字符串处理
来源：http://qbs.pycfn.com

================================================================================
来源：http://etl.wangdashe.top

[E01] 拼接字符串
来源：http://mdv.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hbt.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ndx.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://olc.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dfh.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://psd.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bpg.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://glu.fzhhl.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://avn.jyoumei.cn

[E02] 重复字符串
来源：http://tlz.cheryme.top

Py:   "ab" * 3
来源：http://wuk.gzhubu.top

PHP:  str_repeat("ab", 3);
来源：http://ror.daria6918.cn

JS:   "ab".repeat(3)
来源：http://gyl.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://tso.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://xgu.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://jvm.hfpthk.cn

Ruby: "ab" * 3
来源：http://zru.fehbvm.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rgy.yj20258.top

[E03] 截取子串
来源：http://ack.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tqi.fanxiaobao.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gzk.xuanzx.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oak.fengsongda.top

TS:   s.slice(1, 4)
来源：http://oeq.zdqjudy.top

Java: s.substring(1, 4)
来源：http://cik.fanxiaobao.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qry.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://asq.hammf.cn

C#:   s.Substring(1, 3)
来源：http://ouf.fktsv.cn

[E04] 查找子串位置
来源：http://acd.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://lwk.hcnkem.com

PHP:  strpos($s, "x");
来源：http://scn.yongpay.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fij.hysaishi.cn

TS:   s.indexOf("x")
来源：http://xus.shzxlz.cn

Java: s.indexOf("x")
来源：http://jkw.yongpay.top

Go:   strings.Index(s, "x")
来源：http://cfn.guowangkeji.top

Ruby: s.index("x")
来源：http://fue.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://iqa.shzxlz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://umh.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cgn.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uoh.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hxy.yuanzhike.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zsg.sweek.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vhq.dianchejie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bmz.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://joq.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yrd.shangyingyoupin.top

[E06] 替换子串
来源：http://trw.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qqw.shanyushiyangtech.top

PHP:  str_replace("a", "b", $s);
来源：http://frf.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hnu.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://pps.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yuo.vqdsnc.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ayl.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jfw.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://fkn.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://qzg.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xoq.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pdg.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://tnq.jinghuilouyu.cn

TS:   s.split(",")
来源：http://fmu.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://zzs.zdbjq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lwm.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://bbu.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tgm.bjfxy.top

[E08] 数组按分隔符合并
来源：http://hrs.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://fxf.dianchejie.cn

PHP:  implode(",", $items);
来源：http://hdg.dashuyun.cn

JS:   items.join(",")
来源：http://cyd.sysykeji.top

TS:   items.join(",")
来源：http://xym.vqdsnc.cn

Java: String.join(",", items)
来源：http://lkg.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://yln.daria6918.cn

Ruby: items.join(",")
来源：http://grr.ehwqpu.com

C#:   string.Join(",", items)
来源：http://stb.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://qhg.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uyg.guannengcc.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://exw.gzhubu.top

JS:   s.replace(/\s+/g, "")
来源：http://elx.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://fwj.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://baq.gzhubu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tjl.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://dwo.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rsa.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://kor.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dnb.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fgb.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://nyw.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://hzb.xylfe.cn

Java: String.format("%03d", 7)
来源：http://uqk.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://btp.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xcz.snrcjt.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jha.tarul.cn

[E11] 反转字符串
来源：http://spm.yongpay.top

Py:   s[::-1]
来源：http://eyy.zdqjudy.top

PHP:  strrev($s);
来源：http://ngr.yonumen.top

JS:   [...s].reverse().join("")
来源：http://mdb.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://piy.shanyushiyangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://drw.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://btt.cqqwz.cn

Ruby: s.reverse
来源：http://yvd.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://cqn.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://ubd.epnwcf.com

Py:   s.count("a")
来源：http://rll.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://xpz.cucudq.cn

JS:   s.split("a").length - 1
来源：http://wvf.yongpay.top

TS:   s.split("a").length - 1
来源：http://abw.jqgfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://upw.jyoumei.cn

Go:   strings.Count(s, "a")
来源：http://sol.yanxiufei.cn

Ruby: s.count("a")
来源：http://tgz.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://mag.sxryk.cn

[E13] 逐字符遍历
来源：http://xzu.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://vkv.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mgs.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uxg.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://zqz.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yab.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dbx.hammf.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nlt.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hxo.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://whv.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://noz.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ohn.fanxiaobao.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uoo.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wty.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://syn.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://txz.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mtg.zdbjq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ziu.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://bxq.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sul.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sce.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bmj.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tfr.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pca.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uhp.zhoulong.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xnt.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bcu.shanyushiyangtech.top

[E16] 数字千分位
来源：http://awy.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://epw.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://hox.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dml.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://aao.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://byd.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ezh.shanyushiyangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qob.316326.xyz

C#:   1234567.ToString("N0")
来源：http://yfm.epnwcf.com

[E17] 首字母大写
来源：http://bzo.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nth.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tvn.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nsx.bjfxy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kir.sysykeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://crt.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yyu.nanxuanxn.top

Ruby: s.capitalize
来源：http://awg.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qjr.dashuyun.cn

[E18] 模板占位符替换
来源：http://rwl.yvedp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ylz.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kpt.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vpj.ppjwa.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nie.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gzc.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uub.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pym.yonumen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gyv.shuidangran.top

[E19] 多行文本按行拆分
来源：http://exd.tianlin.xyz

Py:   s.splitlines()
来源：http://zjr.yonumen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sao.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://ekw.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://bzg.yvedp.cn

Java: s.lines().toList()
来源：http://dpp.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://nll.pycfn.com

Ruby: s.lines
来源：http://eot.wangdashe.top

C#:   s.Split('\n')
来源：http://zfk.zycfv.cn

[E20] 判断字符串是否为空
来源：http://riv.haohaochexian.top

Py:   if not s:
来源：http://iqx.shanyushiyangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jew.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://knn.shzxlz.cn

TS:   if (s === "") {}
来源：http://sqt.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://lrh.jinghuilouyu.cn

Go:   if s == "" {}
来源：http://nxx.yangfankeji.com

Ruby: if s.empty?
来源：http://fig.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jvg.tanke756.top

[E21] 超长截断加省略号
来源：http://yrl.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vvv.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uvo.gzhubu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://juv.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fhr.fktsv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fzd.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://mik.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zja.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://grv.ehwqpu.com

[E22] 字节长度与字符长度
来源：http://crx.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fbe.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bfr.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://who.jiagoushi.top


<!-- 参考信息 -->