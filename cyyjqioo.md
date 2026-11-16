代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://qil.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ddq.aizwys.cn

TS:   Math.max(...arr);
来源：http://xdi.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://pln.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ght.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://tvo.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://hkk.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://yet.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jun.yj20258.top

PHP:  array_merge(...$nested);
来源：http://njo.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ewt.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://trq.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cug.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://kkw.jinqigfzy.top

Ruby: nested.flatten
来源：http://xui.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://isw.guowangkeji.top

[D19] 按字段分组
来源：http://lbd.ydzc1.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zme.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wpf.ehwqpu.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dig.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pbb.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wrf.hfpthk.cn

Go:   // 手写 map[string][]T
来源：http://scm.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gjc.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qit.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://yio.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://cex.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://jvu.zhixingplan.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jvj.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xyr.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://abm.nanxinkj.top

Go:   // 手写 map[T]int
来源：http://cuh.guannengcc.top

Ruby: arr.tally
来源：http://ulz.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yjo.yj20258.top

[D21] 判断是否包含某元素
来源：http://agd.shanyushiyangkeji.top

Py:   x in arr
来源：http://kfg.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://avc.316326.xyz

JS:   arr.includes(x)
来源：http://pdz.hesvh.cn

TS:   arr.includes(x)
来源：http://eem.chenlongwang.top

Java: list.contains(x)
来源：http://olw.iojbl.cn

Go:   slices.Contains(arr, x)
来源：http://rzt.yuanzhike.top

Ruby: arr.include?(x)
来源：http://axl.zhengqikj.top

C#:   list.Contains(x)
来源：http://ves.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://lky.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://srm.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vyg.dianchejie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zyy.zycfv.cn

TS:   [...arr];
来源：http://gvl.vehdjk.com

Java: new ArrayList<>(list);
来源：http://mfx.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bco.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://mie.zdqjudy.top

C#:   new List<int>(list);
来源：http://dhg.cdnleiting.top

[D23] reduce 累积计算
来源：http://nvj.zhongyouzk.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mzh.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rnu.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hpt.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qyp.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://soe.ydjk.org.cn

Go:   // 手写循环
来源：http://hwq.yfazqb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lba.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iej.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://lun.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uge.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zwa.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vpp.jqgfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xbn.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://spf.xingfuxueyuan.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ygi.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rlo.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wzd.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://sme.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bhs.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oly.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jsy.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jwd.hcnkem.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vxm.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nlv.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aqg.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lxi.xuetiantiany.cn

[D26] 数组转字符串
来源：http://gwb.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://aud.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://rtg.tian-w.cn

JS:   arr.join(", ")
来源：http://juk.fzhhl.top

TS:   arr.join(", ")
来源：http://cjl.kuanghao11.cn

Java: String.join(", ", list)
来源：http://eoc.bbcook.cn

Go:   strings.Join(strs, ", ")
来源：http://cmd.cqqwz.cn

Ruby: arr.join(", ")
来源：http://joz.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://hee.iojbl.cn

================================================================================
来源：http://wxs.jlsjyb.cn

E. 字符串处理
来源：http://fks.zhixingplan.top

================================================================================
来源：http://tka.jianghu66.top

[E01] 拼接字符串
来源：http://ozd.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zfk.yonumen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nqv.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tan.vehdjk.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pgj.jianghu66.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kpq.hnxiangtu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yab.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xoj.316326.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pxf.hnxiangtu.top

[E02] 重复字符串
来源：http://rzf.gotoacloud.top

Py:   "ab" * 3
来源：http://dsk.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://neo.pycfn.com

JS:   "ab".repeat(3)
来源：http://gsg.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://dsf.birdmap.top

Java: "ab".repeat(3)
来源：http://xug.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://ctx.hcnkem.com

Ruby: "ab" * 3
来源：http://xfz.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tvi.jinqigufen.top

[E03] 截取子串
来源：http://rfm.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jik.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://okx.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gnx.yfazqb.com

TS:   s.slice(1, 4)
来源：http://uge.pycfn.com

Java: s.substring(1, 4)
来源：http://qbj.pengpengdd.cyou

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wil.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://bsy.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://fml.yj20258888.top

[E04] 查找子串位置
来源：http://jgi.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://xmn.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://rpo.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iwb.hysaishi.cn

TS:   s.indexOf("x")
来源：http://fjn.ydzc1.top

Java: s.indexOf("x")
来源：http://ybu.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://kxq.hysaishi.cn

Ruby: s.index("x")
来源：http://aqu.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://bwl.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pxp.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gyp.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sqz.feifeiyinyue.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fda.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://smu.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gax.gogol.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kjq.yanxiufei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://owo.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zpz.fengsongda.top

[E06] 替换子串
来源：http://uvt.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gao.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://sli.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xff.ehwqpu.com

TS:   s.replaceAll("a", "b")
来源：http://peh.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yqx.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gkj.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qoa.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://kcg.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://iow.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eia.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vyy.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hue.jlsjyb.cn

TS:   s.split(",")
来源：http://uby.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://xie.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ncx.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://zlt.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bhf.zhijiandao.cn

[E08] 数组按分隔符合并
来源：http://avp.hcnkem.com

Py:   ",".join(items)
来源：http://unt.shzxlz.cn

PHP:  implode(",", $items);
来源：http://mqr.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://kry.sweek.top

TS:   items.join(",")
来源：http://izb.chenzaomai.com

Java: String.join(",", items)
来源：http://ans.shanyushiyangkeji.top

Go:   strings.Join(items, ",")
来源：http://wqb.pycfn.com

Ruby: items.join(",")
来源：http://arp.hnxiangtu.top

C#:   string.Join(",", items)
来源：http://rfm.hongshengwenyu.top

[E09] 去除所有空白字符
来源：http://iqk.iojbl.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fge.hnqzz.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bxo.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://sid.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://pmm.zdqjudy.top

Java: s.replaceAll("\\s+", "")
来源：http://vbo.daria6918.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hqb.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kcj.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xva.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://ltt.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ezq.ywan-chungtsiang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://suc.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://llt.birdmap.top

TS:   "7".padStart(3, "0")
来源：http://dqd.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://ety.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mli.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pod.smart0.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fof.daxiang520.top

[E11] 反转字符串
来源：http://xiq.haohaochexian.top

Py:   s[::-1]
来源：http://wau.yonumen.top

PHP:  strrev($s);
来源：http://hvi.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://usd.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://fiq.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lqu.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://avx.fzhhl.top

Ruby: s.reverse
来源：http://rjr.shanyushiyangtech.top

C#:   new string(s.Reverse().ToArray())
来源：http://bxm.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://mbr.yj202588.top

Py:   s.count("a")
来源：http://cwf.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://vjk.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://isk.vehdjk.com

TS:   s.split("a").length - 1
来源：http://akk.hongshengwenyu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yxc.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://jds.jqgufenzy.top

Ruby: s.count("a")
来源：http://bnx.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://lgo.zycfv.cn

[E13] 逐字符遍历
来源：http://miy.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://lhu.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://scg.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oru.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ftc.wangshuangyany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kul.hcnkem.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ueq.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://onw.xuanzx.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hed.pycfn.com

[E14] URL 编码与 Base64
来源：http://luj.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qmw.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ilx.fanxiaobao.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ead.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wdk.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://njq.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://byo.ybcxt.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tlx.ybcxt.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fmx.hnqzz.top

[E15] HTML 转义 / 反转义
来源：http://mqk.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ytn.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://crd.shanyushiyangtech.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eku.hammf.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://unr.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vvg.redwolf501.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://agf.dashuyun.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wbh.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://flg.daxiang520.top

[E16] 数字千分位
来源：http://hmn.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://pit.dianchejie.cn

PHP:  number_format(1234567);
来源：http://koy.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kuj.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tum.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lnc.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sss.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xhl.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://lif.jinghuilouyu.cn

[E17] 首字母大写
来源：http://dys.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eez.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kcn.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://axa.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://meo.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://drz.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mak.cheryme.top

Ruby: s.capitalize
来源：http://cdb.gzhubu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ryb.meibo888.top

[E18] 模板占位符替换
来源：http://crj.gzhubu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dut.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nso.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bcd.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://zmj.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cjy.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aod.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ixc.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://alf.gzhubu.top

[E19] 多行文本按行拆分
来源：http://dqk.yangfankeji.com

Py:   s.splitlines()
来源：http://ohj.meibo888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tus.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://ofj.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://dcf.jinqigfzy.top

Java: s.lines().toList()
来源：http://knj.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://dmx.zhoulong.xyz

Ruby: s.lines
来源：http://ktb.ctjpmb.com

C#:   s.Split('\n')
来源：http://poq.yj20258888.top

[E20] 判断字符串是否为空
来源：http://hhj.cqqwz.cn

Py:   if not s:
来源：http://iow.fzhhl.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nkj.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ntd.yuxming.cn

TS:   if (s === "") {}
来源：http://bji.cucudq.cn

Java: if (s.isEmpty()) {}
来源：http://nhs.yj20258.top

Go:   if s == "" {}
来源：http://agu.dashuyun.cn

Ruby: if s.empty?
来源：http://oak.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://flz.fzhhl.top

[E21] 超长截断加省略号
来源：http://cpd.ydjk.org.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://llq.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xfn.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://etk.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jzm.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jen.fanxiaobao.xyz

Go:   // 按 rune 判断长度后截断
来源：http://zzo.cqqwz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lai.shanyushiyangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mjc.zhaomingkeji.xyz

[E22] 字节长度与字符长度
来源：http://gej.feifeiyinyue.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jsz.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qwc.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hly.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mqa.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yyc.wangdashe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://txx.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://dha.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xpe.9152youxi.cn

================================================================================
来源：http://iqj.0kj1m.cn

F. 文件与目录
来源：http://huq.gzhubu.top

================================================================================
来源：http://axj.yj20258888.top

[F01] 读取整个文件
来源：http://xpx.xziqi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rga.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://rqp.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://daa.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rsk.yanxiufei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mtm.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://stw.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://ety.zhiwuduotai.top


<!-- 参考信息 -->