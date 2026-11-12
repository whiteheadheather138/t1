代发 wailian999

TS:   [...new Set(arr)]
来源：http://mkv.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jqc.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://thz.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://hlg.andypj.xyz

C#:   list.Distinct().ToList()
来源：http://fcg.smart0.xyz

[D16] 求和与平均值
来源：http://ynj.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hfq.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dod.xuanzx.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pcc.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lfl.xylfe.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vkm.hnqzz.top

Go:   // 手写循环累加
来源：http://clq.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yni.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://tzq.zhoulong.xyz

[D17] 最大值与最小值
来源：http://qkt.vehdjk.com

Py:   max(arr);  min(arr)
来源：http://xwe.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://dvp.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uqf.birdmap.top

TS:   Math.max(...arr);
来源：http://tgn.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ggo.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lgo.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://dst.shanyushiyangtech.top

C#:   list.Max();  list.Min()
来源：http://gcr.ivvv.top

[D18] 扁平化嵌套数组
来源：http://qgt.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jaz.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://qlb.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pcz.tianlin.xyz

TS:   nested.flat();
来源：http://moy.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nhh.tianlin.xyz

Go:   // 手写双层循环
来源：http://smb.chenzaomai.com

Ruby: nested.flatten
来源：http://xqc.9152youxi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jsy.fehbvm.com

[D19] 按字段分组
来源：http://pqj.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tsv.xingfuxueyuan.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://puk.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dta.vqdsnc.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ltl.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dhe.yonumen.top

Go:   // 手写 map[string][]T
来源：http://era.epnwcf.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://xmb.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wqm.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://xvr.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://foi.cashguo.top

PHP:  array_count_values($arr);
来源：http://lca.yongpay.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fqu.xziqi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ocp.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jsn.birdmap.top

Go:   // 手写 map[T]int
来源：http://ifn.yj20258.top

Ruby: arr.tally
来源：http://btp.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://swu.yonumen.top

[D21] 判断是否包含某元素
来源：http://vmx.zhoulong.xyz

Py:   x in arr
来源：http://vij.zdqjudy.top

PHP:  in_array($x, $arr, true);
来源：http://jmk.daxiang520.top

JS:   arr.includes(x)
来源：http://lfe.yvedp.cn

TS:   arr.includes(x)
来源：http://jgw.nanxuanxn.top

Java: list.contains(x)
来源：http://mew.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://bzb.tianlin.xyz

Ruby: arr.include?(x)
来源：http://cyv.ctjpmb.com

C#:   list.Contains(x)
来源：http://zjg.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://zue.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dne.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mjk.fanxiaobao.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mjj.tianlin.xyz

TS:   [...arr];
来源：http://jdx.nanxuanxn.top

Java: new ArrayList<>(list);
来源：http://jmh.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sqd.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://cye.tian-w.cn

C#:   new List<int>(list);
来源：http://swp.hesvh.cn

[D23] reduce 累积计算
来源：http://hsn.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pff.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sug.yongpay.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mla.jqgufenzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://won.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zcd.jiagoushi.top

Go:   // 手写循环
来源：http://dez.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hvt.guannengcc.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://spr.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://yis.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ynd.uphjek.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ypw.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gvo.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nuw.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xlh.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eiw.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dvs.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oea.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://ygw.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bez.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vui.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ckr.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hel.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://axf.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xid.xziqi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lri.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cop.ctjpmb.com

[D26] 数组转字符串
来源：http://qlk.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://gol.sufxvd.cn

PHP:  implode(", ", $arr);
来源：http://sen.bbcook.cn

JS:   arr.join(", ")
来源：http://rul.shuidangran.top

TS:   arr.join(", ")
来源：http://bop.ybcxt.top

Java: String.join(", ", list)
来源：http://ggi.jinyuanbaomall.cn

Go:   strings.Join(strs, ", ")
来源：http://iqb.jqgufenzy.top

Ruby: arr.join(", ")
来源：http://pxj.xylfe.cn

C#:   string.Join(", ", list)
来源：http://kuk.cqqwz.cn

================================================================================
来源：http://nve.hesvh.cn

E. 字符串处理
来源：http://otg.jinghuilouyu.cn

================================================================================
来源：http://zwt.hnqzz.top

[E01] 拼接字符串
来源：http://lgo.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sji.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tua.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hki.xziqi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xpt.shzxlz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://isl.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jov.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://swj.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ivm.cashguo.top

[E02] 重复字符串
来源：http://fcr.pycfn.com

Py:   "ab" * 3
来源：http://kmd.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://adv.yonumen.top

JS:   "ab".repeat(3)
来源：http://dzp.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://ljr.snrcjt.cn

Java: "ab".repeat(3)
来源：http://lrh.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://pjv.hesvh.cn

Ruby: "ab" * 3
来源：http://umc.svipenyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cxj.tarul.cn

[E03] 截取子串
来源：http://fje.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jib.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jje.iojbl.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bcp.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://zjx.xylfe.cn

Java: s.substring(1, 4)
来源：http://skl.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gys.ehwqpu.com

Ruby: s[1, 3];  s[1..3]
来源：http://nhv.jinghuilouyu.cn

C#:   s.Substring(1, 3)
来源：http://gdq.52xcode.cn

[E04] 查找子串位置
来源：http://wwh.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://pxf.xylfe.cn

PHP:  strpos($s, "x");
来源：http://etq.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://alw.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://bde.zdqjudy.top

Java: s.indexOf("x")
来源：http://uxx.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://ztr.hammf.cn

Ruby: s.index("x")
来源：http://hat.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://fui.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vnl.daria6918.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://twz.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lyf.yanxiufei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ejg.hywenlv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://plb.jinqigfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xhf.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mhx.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bgg.shanyushiyangtech.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sdg.hysaishi.cn

[E06] 替换子串
来源：http://zof.hysaishi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sck.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://lvo.zhengqikj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rtw.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://cfy.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yma.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tvg.52xcode.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://owb.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://sbi.hesvh.cn

[E07] 按分隔符拆分
来源：http://uev.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wkl.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hme.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://njv.ppjwa.cn

TS:   s.split(",")
来源：http://kne.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://rze.jqgfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://njd.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://nzx.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xac.fehbvm.com

[E08] 数组按分隔符合并
来源：http://gxs.xuetiantiany.cn

Py:   ",".join(items)
来源：http://mha.yj20258888.top

PHP:  implode(",", $items);
来源：http://fpr.yuxming.cn

JS:   items.join(",")
来源：http://yml.redwolf501.top

TS:   items.join(",")
来源：http://ekd.ywan-chungtsiang.top

Java: String.join(",", items)
来源：http://qle.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://cpx.yj202588.top

Ruby: items.join(",")
来源：http://hey.zhengqikj.top

C#:   string.Join(",", items)
来源：http://ifs.fktsv.cn

[E09] 去除所有空白字符
来源：http://cqy.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pbo.yj20258888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rgy.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://fhs.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://nxz.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://rah.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://skt.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vgg.52xcode.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tjk.yongpay.top

[E10] 左侧补零 / 定长填充
来源：http://dkq.c1oappe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://clc.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iuw.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://dgt.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://nag.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://bfa.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://dll.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eap.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cju.shanyushiyangtech.top

[E11] 反转字符串
来源：http://qzh.zhengqikj.top

Py:   s[::-1]
来源：http://ccc.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://ktl.svipenyu.cn

JS:   [...s].reverse().join("")
来源：http://lxl.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://tzj.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://akt.sweek.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jfv.bbcook.cn

Ruby: s.reverse
来源：http://zen.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://vod.yvedp.cn

[E12] 统计某字符出现次数
来源：http://fro.xinyue.icu

Py:   s.count("a")
来源：http://skk.fanxiaobao.xyz

PHP:  substr_count($s, "a");
来源：http://ggt.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://kxv.daxiang520.top

TS:   s.split("a").length - 1
来源：http://hit.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lhz.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://cey.sysykeji.top

Ruby: s.count("a")
来源：http://oux.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://zdn.yueranfly.top

[E13] 逐字符遍历
来源：http://nse.shanyushiyangtech.top

Py:   for ch in s: print(ch)
来源：http://arl.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ygk.bbcook.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dtf.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ujq.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jwq.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bls.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xvh.zdqjudy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dkj.zhixingplan.top

[E14] URL 编码与 Base64
来源：http://acj.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://phf.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yvk.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gsa.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bom.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sra.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yko.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xua.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fxs.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://kdy.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rct.gzhubu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://krw.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sml.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eab.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vqp.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ttq.pycfn.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rdy.shangyingyoupin.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ags.zycfv.cn

[E16] 数字千分位
来源：http://ihb.hesvh.cn

Py:   f"{1234567:,}"
来源：http://crt.yvedp.cn

PHP:  number_format(1234567);
来源：http://bxa.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://oxc.yuanzhike.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ngo.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bga.zhiwuduotai.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nfl.jianghu66.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hpu.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://mrc.wangdashe.top

[E17] 首字母大写
来源：http://edf.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tyt.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://nrh.jinghuilouyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ynv.pengpengdd.cyou

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aww.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://shh.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jdw.sysykeji.top

Ruby: s.capitalize
来源：http://mkh.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pol.ehwqpu.com

[E18] 模板占位符替换
来源：http://fsx.shangyingyoupin.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nve.ydjk.org.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dyr.sxryk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yna.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rvq.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bev.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lhm.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ugw.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wsl.quarkkingdee.top

[E19] 多行文本按行拆分
来源：http://vji.jianghu66.top

Py:   s.splitlines()
来源：http://pxx.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mjs.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://jeq.jyoumei.cn

TS:   s.split(/\r?\n/)
来源：http://pdw.chenzaomai.com

Java: s.lines().toList()
来源：http://zww.ydjk.org.cn

Go:   strings.Split(s, "\n")
来源：http://gku.ppjwa.cn

Ruby: s.lines
来源：http://hnd.sweek.top

C#:   s.Split('\n')
来源：http://hds.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://fpo.yangfankeji.com

Py:   if not s:
来源：http://dss.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ocz.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qjc.wangdashe.top

TS:   if (s === "") {}
来源：http://jwp.wangdashe.top

Java: if (s.isEmpty()) {}
来源：http://wcc.haohaochexian.top

Go:   if s == "" {}
来源：http://csu.chenjidiqi.icu

Ruby: if s.empty?
来源：http://eij.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pel.nanxuanxn.top

[E21] 超长截断加省略号
来源：http://slb.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gqu.wangdashe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fns.hnqzz.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://woy.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://grz.gogol.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tfd.yanxiufei.cn

Go:   // 按 rune 判断长度后截断
来源：http://jpx.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fwh.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://stp.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://zlw.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ykh.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xhe.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://viz.hammf.cn


<!-- 参考信息 -->